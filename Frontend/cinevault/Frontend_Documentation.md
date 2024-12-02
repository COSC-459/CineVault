# CineVault Frontend Setup Documentation

This guide provides instructions for setting up the **CineVault** frontend, including prerequisites, commands, and key functionalities.

---

## File Structure

```plaintext
Frontend/
├── cinevault/
│   ├── app/
│   │   ├── Admin/
│   │   ├── Explore/
│   │   ├── Genres/
│   │   ├── Home/
│   │   ├── Login/
│   │   ├── Profile/
│   │   ├── lotties/
│   │   ├── movies/
│   │   ├── constants/
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   ├── globals.css
│   ├── components/
│   │   ├── ui/
│   │   │   ├── avatar.tsx
│   │   │   ├── badge.tsx
│   │   │   ├── button.tsx
│   │   │   ├── card.tsx
│   │   │   ├── dialog.tsx
│   │   │   ├── form.tsx
│   │   │   ├── header.tsx
│   │   │   ├── input.tsx
│   │   │   ├── label.tsx
│   │   │   ├── movieCard.tsx
│   │   │   ├── review.tsx
│   │   │   ├── select.tsx
│   │   │   ├── table.tsx
│   │   │   ├── tabs.tsx
│   │   │   ├── textarea.tsx
│   │   │   ├── sheet.tsx
│   ├── userContext.tsx
│   ├── next.config.js
│   ├── package.json
│   ├── tsconfig.json
│   ├── .eslintrc.json
```

---

## Prerequisites

- **Node.js 16+**
- **npm** or **yarn**

---

## 1. Clone the Repository

```bash
git clone <repository-url>
cd Frontend/cinevault
```bash
cd .. # To navigate to the root directory of the repository
```
```

---

## 2. Install Dependencies

Run the following command to install all required dependencies:

```bash
npm install
```

---

## 3. Environment Variables

Create a `.env.local` file in the root directory for your frontend configuration. Example:

```plaintext
NEXT_PUBLIC_BACKEND_URL=http://127.0.0.1:5000
```

Ensure this URL points to your backend server.

---

## 4. Run the Development Server

Start the Next.js development server:

```bash
npm run dev
```

The server will start at `http://localhost:3000`.

---

## 5. Build for Production

To create a production build:

```bash
npm run build
```

You can then serve the production build locally:

```bash
npm run start
```

---

## Frontend Functionalities

The **CineVault** frontend is powered by **Next.js 15**, **Shadcn**, and **Tailwind CSS**. It features:

### Key Pages:

1. **Home Page**: Displays recent and featured movies.
2. **Explore Page**: Allows users to search and filter movies by title, genre, and actor.
3. **Genres Page**: Lists movies by genres.
4. **Profile Page**: Shows user information, watchlist, and reviews.
5. **Admin Page** (Admin Only): Enables adding, updating, and deleting movies.

### Reusable Components:

- **Headers**: Unified navigation bar.
- **Movie Cards**: Display movie details like poster, title, and rating.
- **Forms and Inputs**: For user input and search functionalities.
- **Modals**: For adding/editing movies and reviews.
- **Tables**: Used in admin pages to manage movies.

---

## Admin Functionality

The **Admin Page** is exclusively accessible to admin users and includes the following:

- **Add Movie**: Add new movies to the database.
- **Update Movie**: Modify movie details, including title, genres, and rating.
- **Delete Movie**: Remove movies from the database.

Admin functionality is determined by the `user_type` field provided by the backend during authentication.

---

By following this guide, you can successfully set up and run the frontend for **CineVault**.

