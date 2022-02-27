# spring-cloud-config-server-using-gitHub-repository

### @EnableConfigServer

This annotation will tell that the application is a configuration server and will enable the configuartion server dependencies.

### @RequestScope

It is used to load the configuration properties value from the Config server.

### @Lazy

By default, Spring creates all singleton beans eagerly at the startup/bootstrapping of the application context. The reason behind this is simple: to avoid and detect all possible errors immediately rather than at runtime.
However, there're cases when we need to create a bean, not at the application context startup, but when we request it.
When we put @Lazy annotation over the @Configuration class, it indicates that all the methods with @Bean annotation should be loaded lazily.
