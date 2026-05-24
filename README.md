# Flutter KK Database Project

This is a Flutter application to manage a database for storing: `Name`, `Nomor KK (16 digit)`, and `Alamat`. The application uses Firebase Firestore as the database and includes CRUD (Create, Read, Update, Delete) and Search functionality.

## Features:

- ✅ Add new data (Create)
- ✅ View existing data (Read)
- ✅ Edit or modify data (Update)
- ✅ Delete data (Delete)
- ✅ Search for specific records

## Technologies Used:

- **Frontend**: Flutter (Dart)
- **Database**: Firebase Firestore

## Project Structure

```
lib/
├── main.dart              # Entry point
├── models/
│   └── person_model.dart  # Data model for person
├── screens/
│   ├── home_screen.dart   # Home/List screen
│   ├── add_screen.dart    # Add new data
│   └── edit_screen.dart   # Edit data
├── services/
│   └── firestore_service.dart  # Firebase operations
└── widgets/
    └── search_widget.dart # Search functionality
```

## Setup Instructions

1. Clone this repository
2. Install Flutter dependencies: `flutter pub get`
3. Set up Firebase project and Firestore database
4. Add your `google-services.json` (Android) and `GoogleService-Info.plist` (iOS)
5. Run: `flutter run`

## Database Schema (Firestore)

Collection: `people`
- `id` (String) - Document ID
- `nama` (String) - Full name
- `nomorKK` (String) - 16 digit KK number
- `alamat` (String) - Address
- `createdAt` (Timestamp) - Creation timestamp
- `updatedAt` (Timestamp) - Last update timestamp
