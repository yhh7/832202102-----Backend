# Code Style Guide

**Source:** This code style guide is based on:

- [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)
- [Oracle's Java Code Conventions](https://www.oracle.com/java/technologies/javase/codeconventions-contents.html)
- [Spring Boot Documentation](https://spring.io/projects/spring-boot)



### CodeStyle:

#### Java:

1. **Indentation**: Use four spaces for indentation to clearly show the structure of the code. Avoid using tabs as they can be interpreted differently by different editors.

2. **Braces**: Place opening braces on the same line as the statement (e.g, `if`, `for`, `while`, etc.). For example:

   ```
   if (condition) {
       // code block
   }
   ```

3. **Line Length**: Keep lines of code under 80-120 characters to ensure readability and to avoid horizontal scrolling.

4. **Variable Naming**: Use camel Case for variable and method names (e.g, `myVariable`). Use Pascal Case for class names (e.g., `MyClass`). Constants should be in uppercase with underscores (e.g, `MY_CONSTANT`).

5. **Imports**: Organize imports in a consistent manner, either alphabetically or by grouping standard library imports separately from third-party imports.

6. **Whitespace**: Use whitespace to improve readability. For example, put a space after commas, and around operators.

7. **Comments**: Write clear and concise comments to explain the purpose of code or to document complex logic. Avoid obvious comments.

8. **Methods**: Keep methods short and focused on a single task. Avoid having too many parameters.

9. **Classes**: Classes should have a single responsibility and be short enough to be understood quickly.

#### Springboot:

Spring Boot is a framework that builds on top of Spring and provides conventions and configurations to simplify the development of standalone, production-grade applications. Here are some specific code style guidelines for Spring Boot applications:

1. **Configuration**: Use `application.properties` or `application.yml` for configuration and follow a consistent naming convention for properties.
2. **Dependency Injection**: Use constructor-based dependency injection for mandatory dependencies and setter or method injection for optional dependencies.
3. **Components**: Name Spring components (e.g., `@Component`, `@Service`, `@Repository`) descriptively to indicate their purpose.
4. **Controllers**: Organize `@RestController` and `@Controller` classes by functionality, and keep controller methods focused on handling HTTP requests and returning responses.
5. **Endpoints**: Use RESTful naming conventions for endpoints and follow a consistent structure for URL mappings.
6. **Exception Handling**: Use `@ControllerAdvice` and `@ExceptionHandler` annotations to handle exceptions across the application in a centralized manner.
7. **Logging**: Use structured logging (e.g., with Logback or Log4j2) and follow a consistent logging level strategy.
8. **Profiles**: Use Spring profiles (`@Profile`) to manage different configurations for different environments (e.g., development, test, production).
9. **Auto-Configuration**: Leverage Spring Boot’s auto-configuration features but be ready to override default settings when necessary.
10. **Testing**: Write unit tests using `@SpringBootTest` and other testing annotations provided by Spring Boot, and ensure a high test coverage.