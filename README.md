# springdoc-openapi-example

just a minimal working example to show an issue with adding WebMvcConfigurationSupport

if you try to run application and then go to http://localhost:8080/swagger-ui/index.html, you'll face an error:

```
Whitelabel Error Page
This application has no explicit mapping for /error, so you are seeing this as a fallback.

Mon May 01 12:14:48 CEST 2023
There was an unexpected error (type=Not Found, status=404).
```

now if you comment or simply delete `com/example/demo/WebMvcConfiguration.java` class, it'll work fine and you're able
to access http://localhost:8080/swagger-ui/index.html
