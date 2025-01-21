# Java Coding Standards

## 1. Naming Conventions
- Use camelCase for variables, methods, and non-final fields.
- Use PascalCase for class and interface names.
- Constants should be in UPPERCASE_WITH_UNDERSCORES.
- Avoid abbreviations and use meaningful names for readability.

## 2. Indentation and Formatting
- Use 4 spaces per indentation level; do not use tabs.
- Place opening braces `{` on the same line as the declaration.
- Limit line length to 100 characters.
- Add a single blank line between methods and sections of code.

## 3. File Structure
- Each class or interface should reside in its own `.java` file.
- Name files to match the public class or interface they contain.
- Use package names to organize files into logical groups.

## 4. Comments and Documentation
- Use Javadoc comments for public classes, methods, and fields.
- Use block comments (`/* */`) for detailed explanations and inline comments (`//`) sparingly.
- Document the purpose, parameters, and return values of methods.

## 5. Imports
- Avoid wildcard imports (e.g., `import java.util.*`).
- Group imports by:
  1. Standard library imports
  2. Third-party library imports
  3. Project-specific imports
- Separate each group with a blank line.

## 6. Error Handling
- Use exceptions for error handling.
- Catch specific exceptions rather than `Exception` or `Throwable`.
- Include meaningful messages when throwing or logging exceptions.
- Use `try`-with-resources for handling closeable resources.

## 7. Code Style
- Follow the Oracle Code Conventions for the Java Programming Language.
- Use tools like Checkstyle or SpotBugs to enforce standards.
- Remove unused variables and imports.

## 8. Testing
- Use JUnit or TestNG for writing and running tests.
- Structure tests in a `src/test/java` directory.
- Name test classes with `Test` suffix, e.g., `UserServiceTest`.
- Ensure unit tests are independent and repeatable.

## 9. Collections and Streams
- Use generics to ensure type safety in collections.
- Prefer `for-each` loops or streams for iteration over collections.
- Use `Optional` to avoid null pointer exceptions.

## 10. Multithreading
- Use thread-safe collections like `ConcurrentHashMap` for shared data.
- Avoid manual thread management; use `ExecutorService` or higher-level abstractions.
- Always synchronize shared mutable data.

## 11. Performance
- Avoid creating unnecessary objects.
- Use StringBuilder for string concatenation in loops.
- Profile and optimize performance-critical sections of the code.

## 12. Version Control
- Exclude `.class` and other build artifacts using `.gitignore`.
- Write meaningful commit messages.
- Follow a consistent branching strategy (e.g., GitFlow).

## 13. Build and Dependencies
- Use a build tool like Maven or Gradle for dependency management.
- Define dependencies explicitly in `pom.xml` or `build.gradle`.
- Avoid hardcoding version numbers; use a properties file if needed.
