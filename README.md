
# Getting Started with APIMATIC Calculator

## Introduction

Simple calculator API hosted on APIMATIC

## Install the Package

Install the SDK by adding the following dependency in your project's pom.xml file:

```xml
<dependency>
  <groupId>io.sdks</groupId>
  <artifactId>java-pack-sdk</artifactId>
  <version>1.2.3</version>
</dependency>
```

You can also view the package at:
https://central.sonatype.com/artifact/io.sdks/java-pack-sdk/1.2.3

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| `environment` | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| `httpClientConfig` | [`Consumer<HttpClientConfiguration.Builder>`](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |

The API client can be initialized as follows:

```java
APIMATICCalculatorClient client = new APIMATICCalculatorClient.Builder()
    .httpClientConfig(configBuilder -> configBuilder
            .timeout(0))
    .environment(Environment.PRODUCTION)
    .build();
```

## List of APIs

* [Simple Calculator](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/controllers/simple-calculator.md)

## Classes Documentation

* [Utility Classes](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/utility-classes.md)
* [HttpRequest](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/http-request.md)
* [HttpResponse](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/http-response.md)
* [HttpStringResponse](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/http-string-response.md)
* [HttpContext](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/http-context.md)
* [HttpBodyRequest](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/http-body-request.md)
* [HttpCallback Interface](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/http-callback-interface.md)
* [Headers](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/headers.md)
* [ApiException](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/api-exception.md)
* [Configuration Interface](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/configuration-interface.md)
* [HttpClientConfiguration](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/http-client-configuration.md)
* [HttpClientConfiguration.Builder](https://www.github.com/Syed-Subtain/java-pack-java-sdk/tree/1.2.3/doc/http-client-configuration-builder.md)

