---
layout: default
title: Home
nav_order: 1
description: "Documentation for the testing frameworks"
permalink: /
---

# Test Frameworks
{: .fs-9 }

Though Wave and Stream are automation libraries, they are not testing frameworks and cannot create tests by themselves. 
Tests should be created with a test framework like TestNG, Junit, Cucumber etc... This documentation contains the information
about the testing libraries and their custom settings which can be used along with. 
{: .fs-5 .fw-350 }

## TestNG Framework

TestNG is a testing framework inspired from JUnit and NUnit but introducing some new functionalities that make it more powerful and easier to use, such as:

1. Annotations.
2. Run your tests in arbitrarily big thread pools with various policies available (all methods in their own thread, one thread per test class, etc...).
3. Test that your code is multithread safe.
4. Flexible test configuration.
5. Support for data-driven testing (with @DataProvider).
6. Support for parameters.
7. Powerful execution model (no more TestSuite).
8. Supported by a variety of tools and plug-ins (Eclipse, IDEA, Maven, etc...).
9. Embeds BeanShell for further flexibility.
10. Default JDK functions for runtime and logging (no dependencies).
11. Dependent methods for application server testing.

TestNG is designed to cover all categories of tests: unit, functional, end-to-end, integration, etc...

[Cited from TestNG Website]

## Cucumber Framework

Cucumber framework promotes a shared understanding of features and their expected behaviors through scenarios written in the BDD format.


### Dependencies



### To start add the following Maven dependency to your pom.xml file

```xml
        <dependency>
            <groupId>io.github.tidal-code</groupId>
            <artifactId>test</artifactId>
            <version>1.1.0</version>
        </dependency>
```

{: .pt-4 }
Tidal is hosted with [Maven Central](https://mvnrepository.com/artifact/io.github.tidal-code/test){:target='_blank'}. For detailed version information, check the 'Versions' page under the 'Detailed Docs' section. 


For projects using Gradle,
```yml
implementation group: 'io.github.tidal-code', name: 'test', version: '1.1.0'
```

<br>
Please read the [Detailed-Docs]({{ site.url }}/docs/detailed-docs) section to know more about Tidal.TEST

<!-- ### Contributing

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change. Read more about becoming a contributor in [our GitHub repo](https://github.com/tidal-code/Wave#readme). -->


<!-- #### Thank you to the contributors of Just the Docs!

<ul class="list-style-none">
{% for contributor in site.github.contributors %}
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"/></a>
  </li>
{% endfor %}
</ul> -->

<!-- ### Code of Conduct

Just the Docs is committed to fostering a welcoming community.

[View our Code of Conduct](https://github.com/pmarsceill/just-the-docs/tree/master/CODE_OF_CONDUCT.md) on our GitHub repository. -->
