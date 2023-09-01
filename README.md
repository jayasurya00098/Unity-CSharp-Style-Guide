# Unity C# Style Guide

## Introduction

A C# style guide supports the work of developers and the growth of projects. The goal is to have a cleaner, more scalable code base that makes it easier to grow your team and game. This guide provides an overview of the guidelines and examples for developing and maintaining your own style guide.

**Note**: These recommendations are based on general industry standards for C# and are meant to be inspirational rather than rules set in stone. Adapt anything here to your needs and preferences.

## 1. Naming

### General Guidelines:
- Names should be descriptive, clear, and unambiguous.
- Avoid using too many prefixes or special encoding.
- Make names easily searchable.

### Variables:
- Variables should be nouns.
- Prefix booleans with a verb (e.g., `isPlayerSafe`).

### Access Level Modifiers:
- Decide as a team whether to omit access level modifiers or to specify them.

### Casing:
- Local variables and method parameters should be in camelCase.
- Public fields, class, and method names should be in PascalCase.

### Classes:
- Use PascalCase nouns for class names.
- Make class names indicative of their purpose (e.g., `PetFollowController`).

### Methods:
- Start method names with a verb.
- Use camelCase for method parameters.
- Methods returning a boolean should ask questions (e.g., `IsStarving`).

### Events:
- Name events with verb phrases.
- Use present or past participle to indicate events before or after (e.g., `OpeningDoor` or `OpenedDoor`).
- Use the `System.Action` delegate for events.
- Prefix the event raising method with "on" (e.g., `OnOpeningDoor`).

### Namespaces:
- Use PascalCase without symbols or underscores.
- Create sub-namespaces using the dot operator.

## 2. Formatting

### Properties:
- Use expression-bodied syntax for single-line read-only properties.
- Encapsulate data using properties to hide it from unwanted changes.

### Script Serialization:
- Group data in serializable classes or structs to clean up the inspector.
- Use the `SerializeField` attribute for private or protected variables to make them appear in the inspector.
- Use the `Range` attribute to set minimum and maximum values.

### Indentation:
- Use the Allman style from the Microsoft framework design guidelines.
- Don't omit braces, even for single-line statements.

### Spacing:
- Add spaces to decrease code density.
- Use a single space before flow control conditions.
- Add a space before and after comparison operators.

## 3. Classes

### Size:
- Classes should be small and focused.
- Follow the single responsibility principle.

### Refactoring:
- Separate out distinct functionalities into their own classes.
- Use scriptable objects for data.

## 4. Methods

### Size & Responsibility:
- Methods should be small with a single responsibility.
- Each method should describe one action or answer one question.

### Avoid Duplication:
- Follow the DRY (Don't Repeat Yourself) principle.
- Refactor methods to avoid duplicate or repetitious logic.

## Conclusion

Clean code should always look like it was written by someone who cares. Caring is not a destination; it's a daily practice.

For a more detailed style sheet and additional resources, refer to the [Unity eBook](https://on.unity.com/45rvCUX).
