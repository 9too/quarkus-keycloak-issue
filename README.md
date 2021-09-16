```
./gradlew quarkusDev

> Task :quarkusGenerateCode UP-TO-DATE
> Task :compileJava UP-TO-DATE
> Task :processResources UP-TO-DATE
> Task :classes UP-TO-DATE
> Task :processTestResources NO-SOURCE
> Task :quarkusGenerateCodeTests UP-TO-DATE
> Task :compileTestJava NO-SOURCE
> Task :testClasses UP-TO-DATE

> Task :quarkusDev
Listening for transport dt_socket at address: 5005
Press [h] for more options>
2021-09-16 17:34:22,171 INFO  [org.tes.doc.DockerClientProviderStrategy] (build-38) Loaded org.testcontainers.dockerclient.UnixSocketClientProviderStrategy from ~/.testcontainers.properties, will try it first
2021-09-16 17:34:22,458 INFO  [org.tes.doc.DockerClientProviderStrategy] (build-38) Found Docker environment with local Unix socket (unix:///var/run/docker.sock)
2021-09-16 17:34:22,460 INFO  [org.tes.DockerClientFactory] (build-38) Docker host IP address is localhost
2021-09-16 17:34:22,479 INFO  [org.tes.DockerClientFactory] (build-38) Connected to docker:
  Server Version: 20.10.7
  API Version: 1.41
  Operating System: Gentoo/Linux
  Total Memory: 31993 MB
2021-09-16 17:34:22,481 INFO  [org.tes.uti.ImageNameSubstitutor] (build-38) Image name substitution will be performed by: DefaultImageNameSubstitutor (composite of 'ConfigurationFileImageNameSubstitutor' and 'PrefixingImageNameSubstitutor')
2021-09-16 17:34:23,012 INFO  [org.tes.DockerClientFactory] (build-38) Ryuk started - will monitor and terminate Testcontainers containers on JVM exit
2021-09-16 17:34:23,013 INFO  [org.tes.DockerClientFactory] (build-38) Checking the system...
2021-09-16 17:34:23,013 INFO  [org.tes.DockerClientFactory] (build-38) ✔︎ Docker server version should be at least 1.6.0
2021-09-16 17:34:23,070 INFO  [org.tes.DockerClientFactory] (build-38) ✔︎ Docker environment should have more than 2GB free disk space
2021-09-16 17:34:23,081 INFO  [🐳 .io/.0.0]] (build-38) Creating container for image: quay.io/keycloak/keycloak:14.0.0
2021-09-16 17:34:23,121 INFO  [🐳 .io/.0.0]] (build-38) Starting container with ID: 53575b1c30efd32a164a1acbf8f0b76293d4654923cfe9d65ff7fc7b148eb635
2021-09-16 17:34:23,454 INFO  [🐳 .io/.0.0]] (build-38) Container quay.io/keycloak/keycloak:14.0.0 is starting: 53575b1c30efd32a164a1acbf8f0b76293d4654923cfe9d65ff7fc7b148eb635
2021-09-16 17:34:23,461 WARN  [org.tes.con.wai.str.HttpWaitStrategy] (build-38) Unexpected error occurred - will proceed to try to wait anyway: java.lang.IllegalStateException: Target port 1337 is not exposed
	at org.testcontainers.containers.wait.strategy.HttpWaitStrategy.lambda$waitUntilReady$2(HttpWaitStrategy.java:197)
	at java.base/java.util.Optional.orElseThrow(Optional.java:408)
	at org.testcontainers.containers.wait.strategy.HttpWaitStrategy.waitUntilReady(HttpWaitStrategy.java:197)
	at org.testcontainers.containers.wait.strategy.AbstractWaitStrategy.waitUntilReady(AbstractWaitStrategy.java:35)
	at org.testcontainers.containers.GenericContainer.waitUntilContainerStarted(GenericContainer.java:892)
	at org.testcontainers.containers.GenericContainer.tryStart(GenericContainer.java:440)
	at org.testcontainers.containers.GenericContainer.lambda$doStart$0(GenericContainer.java:325)
	at org.rnorth.ducttape.unreliables.Unreliables.retryUntilSuccess(Unreliables.java:81)
	at org.testcontainers.containers.GenericContainer.doStart(GenericContainer.java:323)
	at org.testcontainers.containers.GenericContainer.start(GenericContainer.java:311)
	at io.quarkus.oidc.deployment.devservices.keycloak.KeycloakDevServicesProcessor.startContainer(KeycloakDevServicesProcessor.java:236)
	at io.quarkus.oidc.deployment.devservices.keycloak.KeycloakDevServicesProcessor.startKeycloakContainer(KeycloakDevServicesProcessor.java:128)
	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.base/java.lang.reflect.Method.invoke(Method.java:566)
	at io.quarkus.deployment.ExtensionLoader$2.execute(ExtensionLoader.java:820)
	at io.quarkus.builder.BuildContext.run(BuildContext.java:277)
	at org.jboss.threads.ContextHandler$1.runWith(ContextHandler.java:18)
	at org.jboss.threads.EnhancedQueueExecutor$Task.run(EnhancedQueueExecutor.java:2449)
	at org.jboss.threads.EnhancedQueueExecutor$ThreadBody.run(EnhancedQueueExecutor.java:1478)
	at java.base/java.lang.Thread.run(Thread.java:829)
	at org.jboss.threads.JBossThread.run(JBossThread.java:501)
```
