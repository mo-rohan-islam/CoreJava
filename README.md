# CoreJava
Learning Core Java with Java 8

## Overview

This repository contains example programs and exercises for learning core Java concepts (Java 8). It is organized by topic (collections, concurrency, I/O, OOP concepts, etc.) with small demo programs and assignments under each folder.

## Repository structure

- Each top-level folder (for example, `Abstraction`, `Collections`, `MultiThreading`) contains a `src` directory with Java source files organized by topic and package.
- Use the folders as self-contained examples to study individual language features.

## Build & Run

Quick compile and run from repository root (Windows PowerShell / Command Prompt):

```
javac -d out -sourcepath src $(Get-ChildItem -Recurse -Filter "*.java" -Path .\**\src | ForEach-Object { $_.FullName })
java -cp out fully.qualified.MainClass
```

Or compile a single example and run it:

```
javac -d out src/Collections/src/com/example/CollectionsDemo.java
java -cp out com.example.CollectionsDemo
```

Replace `fully.qualified.MainClass` with the class you want to run (package + class name).

## Contributing

Feel free to add examples, exercises, or improvements. Keep files organized under the appropriate topical folder.

## License

See the repository `LICENSE` file for license details.
