# .NET Coding Standards

## 1. Naming Conventions
- Use PascalCase for class, method, and property names.
- Use camelCase for local variables and parameters.
- Prefix interfaces with an `I` (e.g., `IService`).
- Use meaningful and descriptive names; avoid abbreviations.

## 2. Code Layout
- Use 4 spaces per indentation level.
- Place braces `{}` on a new line for classes, methods, and properties.
- Use a single blank line to separate methods and logical code blocks.

## 3. File Organization
- Place one class, interface, or struct per file.
- Name the file after the class or interface it contains.
- Organize files into folders based on functionality or feature.

## 4. Error Handling
- Use `try`...`catch` blocks to handle exceptions, and log meaningful messages.
- Avoid catching `System.Exception`; catch specific exceptions instead.
- Use `using` statements for resources that need disposal.

## 5. LINQ
- Prefer LINQ over loops for readability when dealing with collections.
- Use query syntax or method syntax consistently within a project.

## 6. Async/Await
- Use `async` and `await` for asynchronous operations.
- Suffix async methods with `Async` (e.g., `GetDataAsync`).
- Avoid blocking asynchronous code by using `.Result` or `.Wait()`.

## 7. Testing
- Use a testing framework like MSTest, NUnit, or xUnit.
- Organize tests in separate projects or directories.
- Name test methods clearly, e.g., `MethodName_StateUnderTest_ExpectedBehavior`.

## 8. Documentation
- Use XML comments to document public methods, properties, and classes.
- Include summary, parameters, and return details in the documentation.
- Enable XML documentation generation in the project settings.

## 9. Code Style
- Use tools like `StyleCop` or `ReSharper` to enforce coding standards.
- Follow the official .NET coding conventions for consistency.

## 10. Dependency Injection
- Use dependency injection to manage dependencies and improve testability.
- Prefer constructor injection over property injection.

## 11. Configuration
- Store configuration in appsettings.json or environment variables.
- Use strongly-typed configuration classes for better maintainability.

## 12. Version Control
- Exclude `bin/`, `obj/`, and other temporary files using `.gitignore`.
- Use descriptive commit messages and branch names.
- Follow GitFlow or a similar branching strategy.
ChatGPT says: The document has been updated with .NET-specific coding standards. Let me know if there are any other adjustments or additional content you'd like to include!
