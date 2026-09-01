# Coffee Shop

A Coffee Shop app built with Kotlin, with some Java, and Firebase, focused on UI design, created as a quick project to test item addition to the cart functionality.


## Features

 * **Premium UI:** Visually appealing, user-friendly, and attractively designed interface for an enhanced user experience.
 * **Popular Coffees:**
   * Users can check coffee ratings.
   * Users can select coffee sizes.
   * Users can add their favorite coffee to the cart.
 * **Cart Screen:**
   * View all items added to the cart with individual prices.
      * Check the subtotal price of all items.
      * Check the delivery charges applied to the order.
      * Can check the total tax on items.
      * Check the total price for the entire order.


## Getting Started

#### 1. [Setup Android Studio](https://developer.android.com/studio)

#### 2. Clone the Repo

```
$ git clone https://github.com/abhinavj4321/MyCoffeeApp
$ cd Coffee-Shop/
```

#### 3. Setup Firebase Realtime Database

1. Create a Firebase Project:
    - Go to the [Firebase Console](https://console.firebase.google.com/) and create a new project.
2. Enable Firebase Realtime Database:
    - In your Firebase project console:
      - Click on Realtime Database from the left-hand menu.
      - Click on "Create Database."
      - Choose "Start in test mode" for initial setup and click "Enable."
3. Add Data to Realtime Database:
    - Download the provided [database_firebase.json](https://github.com/HaroonBsf/Coffee-Shop/releases/download/v1.0.0/database_firebase.json) file.
    - Go to the Firebase Realtime Database in the console.
    - Click on the three dots in the upper right corner and select Import JSON.
    - Choose the `database_firebase.json` file and import it to populate the database with initial data.

#### 4. Configure Firebase for Android

1. Create an Android App in Firebase:
    - In the Firebase console, go to **Project settings**.
    - Under "Your apps," select **Add app** and choose **Android**.
    - Enter your package name (e.g., com.yourname.coffeeshopapp).
2. Download and Add `google-services.json:`
    - Follow the on-screen instructions in Firebase to download the google-services.json file.
    - Place it in your project’s `/app` directory.
3. Add SHA-1 Key:
    - Run the following command to get your SHA-1 key:
      
      ```
      keytool -exportcert -list -v -alias androiddebugkey -keystore ~/.android/debug.keystore
      ```
    - In the Firebase console, under the Android app settings, add your SHA-1 key by clicking "Add Fingerprint."

#### 5. Add Dependencies
  - Check and add the latest versions of the necessary dependencies for Firebase Realtime Database, Lifecycle (extensions, ViewModel, LiveData, runtime), Glide, and Gson to your project.
  - For detailed instructions on setting up Firebase Realtime Database dependencies, refer to the [Firebase Realtime Database Setup Guide](https://firebase.google.com/docs/database/android/start).
  - Ensure View Binding is enabled. If not, add the following inside the `android` block in your `build.gradle` file (Module: app):
    
    ```
    buildFeatures{
        viewBinding = true
    }
    ```
  - Sync your project with Gradle to ensure all dependencies are correctly added.

#### 6. Final Step
  - Build and run the app on your Android device or emulator.
