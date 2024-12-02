# CineVault Application Overview

CineVault is a full-stack movie management and discovery application designed to provide a seamless user experience for browsing, managing, and reviewing movies. This document highlights the app's features, the technologies used, and its key components.

---

## Features of CineVault

### For Users:
1. **Home Page**:
   - Displays a curated selection of recent and featured movies.
   - Fetches movie data dynamically from the backend.

2. **Explore Page**:
   - Allows users to search and filter movies by title, genre, and actor.
   - Provides an intuitive interface for exploring a large database of movies.

3. **Genres Page**:
   - Organizes movies by genre.
   - Easy navigation to explore movies in specific categories.

4. **Profile Page**:
   - Displays the user's information, watchlist, and submitted reviews.
   - Users can manage their movie watchlists and view detailed reviews.

5. **Watchlist Management**:
   - Add or remove movies from the personal watchlist.
   - Integrated with the backend for real-time updates.

### For Admins:
1. **Admin Page**:
   - Restricted to admin users based on user type.
   - Admins can:
     - Add new movies to the database.
     - Update existing movie details (e.g., title, genres, rating).
     - Delete movies from the database.

2. **Secure Access**:
   - Admin functionality is secured through backend authentication.
   - Admin privileges are assigned via the `user_type` field in the database.

---

## Tech Stack

### Frontend:
1. **Next.js 15**:
   - Provides server-side rendering and efficient page routing.
   - Enhances the performance and SEO of the application.

2. **Shadcn**:
   - Component library for building a cohesive UI.
   - Simplifies the creation of reusable, accessible, and customizable components.

3. **Tailwind CSS**:
   - Utility-first CSS framework for rapid UI development.
   - Enables consistent and responsive designs throughout the app.

### Backend:
1. **Flask**:
   - Lightweight Python web framework for building APIs.
   - Handles authentication, movie data management, and watchlist operations.

2. **PostgreSQL**:
   - Relational database for storing users, movies, genres, reviews, and watchlists.

3. **SQLAlchemy**:
   - ORM for database modeling and interaction.
   - Simplifies complex database queries and associations.

---

## How It Works

1. **Authentication**:
   - Users can log in or register through the backend.
   - Admins have exclusive access to the Admin Page to manage movie data.

2. **Dynamic Movie Data**:
   - The backend provides endpoints for fetching, adding, updating, and deleting movies.
   - Users can view detailed information about movies, including genres, actors, and reviews.

3. **Watchlist Integration**:
   - Users can manage their watchlists in real-time.
   - Watchlist updates are reflected immediately in the user’s profile.

4. **Admin Privileges**:
   - Admins can add new movies via forms on the Admin Page.
   - Movie updates and deletions are securely managed through backend endpoints.

---

## Summary

CineVault combines a feature-rich frontend with a robust backend to deliver an efficient and enjoyable movie management experience. The application leverages modern technologies like **Next.js**, **Tailwind CSS**, and **Flask** to ensure high performance, scalability, and user satisfaction. Whether exploring movies or managing them as an admin, CineVault offers a streamlined interface tailored to