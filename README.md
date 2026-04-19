# In-Class Activity 07: Flutter SQLite (Local Storage Part 1)

A Flutter app that demonstrates local data persistence using SQLite via the `sqflite` package. Covers full CRUD operations and Part 2 challenge features.

## Features

- **Insert** - add a new record to the local database
- **Query All** - retrieve and print all stored records
- **Update** - modify an existing record by ID
- **Delete Last** - remove the most recent record
- **Query by ID** - look up a specific record by its primary key
- **Delete All** - clear the entire table

## Project Structure

```
lib/
├── main.dart             # UI with buttons wired to all CRUD operations
└── database_helper.dart  # Singleton class managing SQLite database access
```

## Dependencies

```yaml
sqflite: ^2.2.2
path_provider: ^2.0.11
path: ^1.8.2
```

## Getting Started

1. Clone the repo
2. Run `flutter pub get`
3. Launch an emulator or connect a device
4. Run `flutter run`
5. Tap buttons and watch output in the **Debug Console**

## How It Works

`DatabaseHelper` opens (or creates) a `.db` file in the device's documents directory on first launch. All subsequent app runs reconnect to the same file, providing true data persistence across sessions.
