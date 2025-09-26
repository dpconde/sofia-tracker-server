# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Sofia Tracker is a Spring Boot application written in Kotlin. It's a server application currently in early development (version 0.0.1-SNAPSHOT).

**Key Details:**
- Package name: `com.dpconde.sofia_tracker` (note: uses underscore instead of hyphen due to Java naming conventions)
- Java/Kotlin version: 17
- Spring Boot version: 3.5.6
- Build tool: Gradle with Kotlin DSL

## Common Development Commands

### Building and Running
```bash
# Build the project
./gradlew build

# Run the application
./gradlew bootRun

# Clean build
./gradlew clean build
```

### Testing
```bash
# Run all tests
./gradlew test

# Run tests with more details
./gradlew test --info

# Run a specific test class
./gradlew test --tests "com.dpconde.sofia_tracker.SofiaTrackerApplicationTests"
```

### Other Useful Commands
```bash
# Check dependencies
./gradlew dependencies

# Generate wrapper (if needed)
./gradlew wrapper
```

## Project Structure

```
src/
├── main/
│   ├── kotlin/com/dpconde/sofia_tracker/
│   │   └── SofiaTrackerApplication.kt    # Main Spring Boot application
│   └── resources/
│       └── application.properties        # Spring configuration
└── test/
    └── kotlin/com/dpconde/sofia_tracker/
        └── SofiaTrackerApplicationTests.kt # Basic context load test
```

## Architecture Notes

- **Framework**: Spring Boot 3.x with Kotlin
- **Testing**: JUnit 5 platform with Spring Boot Test
- **Build**: Standard Gradle project structure
- **Main Class**: `SofiaTrackerApplication.kt` - standard Spring Boot entry point
- **Package Structure**: Currently minimal with just the main application class

This is a new project with basic Spring Boot scaffolding. The architecture will evolve as features are added.