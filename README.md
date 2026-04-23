# Medicine LemonSoft 💊

Medicine LemonSoft is a user-friendly Android application designed to provide quick and easy access to a comprehensive database of medicinal information. Whether you are a healthcare professional or a curious consumer, this app helps you find essential details about various medicines, including brand names, strengths, forms, and unit prices.

## 🚀 Features

- **Searchable Database**: Quickly find medicines by brand name using the real-time search functionality.
- **Detailed Information**: View key details for each medicine:
  - **Brand Name**
  - **Strength** (e.g., 500mg, 10ml)
  - **Form** (e.g., Tablet, Syrup, Injection)
  - **Unit Price** (in BDT)
- **Modern UI**: Clean and intuitive interface built with Material Design components.
- **Offline Access**: Uses a pre-packaged SQLite database, allowing the app to function without an internet connection.
- **Navigation Drawer**: Easy access to different sections of the app (Home, Profile, Settings).

## 🛠️ Tech Stack

- **Platform**: Android
- **Language**: Java
- **Database**: SQLite (managed via `SQLiteAssetHelper`)
- **UI Framework**: Android XML with Material Design 3
- **Build System**: Gradle

## 📂 Project Structure

```text
MedicineApp/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/medicinelemonsoft/
│   │   │   │   ├── MainActivity.java      # Main entry point and search logic
│   │   │   │   ├── MedicineAdepter.java   # RecyclerView adapter for medicine list
│   │   │   │   ├── MedicineModel.java     # Data model for medicine objects
│   │   │   │   └── MedicineSqlite.java    # SQLite database helper
│   │   │   ├── assets/databases/          # Contains the pre-filled medicine.db
│   │   │   ├── res/                       # Layouts, strings, and drawable resources
│   │   │   └── AndroidManifest.xml        # App configuration
│   └── build.gradle                       # App-level dependencies
├── build.gradle                           # Project-level configuration
└── settings.gradle                         # Project settings
```

## ⚙️ Setup & Installation

Follow these steps to get the project running on your local machine:

### Prerequisites

- **Android Studio** (Koala or newer recommended)
- **Java Development Kit (JDK)** 11 or higher
- **Android SDK** (API 34 recommended)

### Steps

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Bisu7/MedicineApp.git
   ```
2. **Open in Android Studio**:
   - Launch Android Studio.
   - Select **Open** and navigate to the `MedicineApp` folder.
3. **Sync Gradle**:
   - Wait for Android Studio to finish indexing and syncing the Gradle files. Ensure you have an active internet connection for this step to download dependencies.
4. **Run the App**:
   - Connect an Android device via USB or start an Emulator.
   - Click the **Run** button (green play icon) in the toolbar.

## 📊 Database Management

The application uses a pre-populated SQLite database located at `app/src/main/assets/databases/medicine.db`.
- To update the medicine list, you can replace this file with a new `.db` file containing the same schema.
- The app uses `SQLiteAssetHelper` to manage the initial deployment of the database from the assets folder to the app's internal storage.

## 🤝 Contributing

Contributions are welcome! If you'd like to improve the app or add new features, please:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a Pull Request.

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details (if applicable).

---
*Developed with ❤️ by the Medicine LemonSoft Team.*
