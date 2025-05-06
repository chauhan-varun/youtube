# YouTube Clone

![Project Screenshot](image.png)

## Overview

A React-based YouTube clone frontend application that uses the YouTube API from RapidAPI. This project features a responsive design with video browsing, search functionality, and video playback capabilities.

**Live Demo:** [https://adfreeyoutube.onrender.com](https://adfreeyoutube.onrender.com)

> **Note:** The live link might not work at the time you open it due to API request limits. To use the application locally, set up your own API key as described below.

## Features

- Home page with trending videos
- Video search functionality
- Video playback with details
- Responsive design for various screen sizes

## Tech Stack

- **Frontend Framework:** React.js
- **Build Tool:** Vite
- **Styling:** Tailwind CSS
- **Routing:** React Router DOM
- **Video Player:** React Player
- **API Handling:** Axios
- **Other Libraries:**
  - js-abbreviation-number (for formatting numbers)
  - moment (for date/time formatting)
  - react-icons
  - react-avatar

## API Integration

This project uses the YouTube API from RapidAPI. You need to obtain an API key from:
[https://rapidapi.com/hub](https://rapidapi.com/hub)

Specifically, it uses the YouTube v3 API: `youtube138.p.rapidapi.com`

## Setup Instructions

1. **Clone the repository**

2. **Install dependencies**
   ```
   npm install
   ```

3. **Set up environment variables**
   - Create a `.env` file in the root directory based on `.env.example`
   - Add your RapidAPI key:
     ```
     VITE_YOUTUBE_API_KEY=your_rapidapi_key_here
     ```

4. **Start the development server**
   ```
   npm run dev
   ```

5. **Build for production**
   ```
   npm run build
   ```

## Project Structure

- `/src/components` - React components for the UI
- `/src/context` - Context providers for state management
- `/src/utils` - Utility functions including API configuration
- `/src/loader` - Loading components

## Routes

- `/` - Home page with trending videos
- `/search/:searchQuery` - Search results page
- `/video/:id` - Video playback page
