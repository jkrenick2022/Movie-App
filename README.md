# Movie App

## Overview

The **Movie App** is a React-based web application that allows users to search for movies and view trending movies. It fetches data from **The Movie Database (TMDB) API** and tracks search queries using **Appwrite**.

## Features

### 🔍 Movie Search
- Users can search for movies using a **search bar**.
- Implements **debouncing** to minimize API requests and improve performance.
- Fetches and displays search results dynamically.

### 📈 Trending Movies
- Displays a list of **trending movies** fetched from TMDB.
- Automatically loads trending movies when the app starts.

### 📊 Search Count Tracking
- Integrates **Appwrite** to store and track search queries.
- Updates the search count each time a user searches for a movie.

### ⚡ Optimized API Calls
- Uses **debouncing** (via `react-use`) to reduce the number of API calls.
- Fetches movie details only when the user has stopped typing for 500ms.

### 🎨 Responsive UI
- Displays movies with their **poster images**.
- Handles errors gracefully with error messages.
- Includes a **spinner** when loading data.

## Tech Stack

- **Frontend:** React, JavaScript
- **State Management:** React Hooks (`useState`, `useEffect`)
- **Debouncing:** `react-use`
- **API:** TMDB API (The Movie Database)
- **Database:** Appwrite (for tracking search queries)
- **Styling:** CSS (Tailwind)

## Installation & Setup

### 1. Clone the Repository
```sh
git clone https://github.com/your-username/Movie-App.git
cd Movie-App
```

### 2. Install Dependencies
```sh
npm install
```

### 3. Set up Environment Variables
- Create a .env file in the root directory.
- Add the following:
```sh
VITE_TMDB_API_KEY=your_tmdb_api_key
VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
```

### 4. Start the Development Server
```sh
npm run dev
```

### 5. Build for Production
```sh
npm run build
```

## Usage
- Search for Movies: Enter a movie name in the search bar.
- View Trending Movies: Check the "Trending Movies" section.
- Track Search Counts: Each search updates the database.

## License
This project is open-source and available under the MIT License.
