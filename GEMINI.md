# Movie Explorer - Project Context

This project is a React-based web application that allows users to explore movies using the TMDB API. It features search, sorting, and pagination.

## Project Overview

- **Main Technologies:** React 19, Vite 8, pnpm.
- **API:** The Movie Database (TMDB) API.
- **Architecture:** A single-page application (SPA) with a main `App.jsx` component managing state for movies, search queries, sorting, and pagination.
- **Key Features:**
  - Search with debouncing (500ms).
  - Sorting by popularity, release date, and rating.
  - Pagination for browsing multiple pages of results.
  - Responsive movie grid layout.

## Building and Running

The project uses `pnpm` as the package manager.

- **Start Development Server:**
  ```bash
  cd movie-explorer
  pnpm dev
  ```
- **Build for Production:**
  ```bash
  cd movie-explorer
  pnpm build
  ```
- **Lint Code:**
  ```bash
  cd movie-explorer
  pnpm lint
  ```
- **Preview Production Build:**
  ```bash
  cd movie-explorer
  pnpm preview
  ```

## Configuration

- **Environment Variables:** Requires a `.env` file in the `movie-explorer` directory with:
  ```
  VITE_TMDB_API_KEY=your_api_key_here
  ```
- **Vite Config:** Configured with a base path `/CS349-H3/` for deployment (likely GitHub Pages).
- **ESLint:** Uses a flat configuration file (`eslint.config.js`) with React Hooks and React Refresh plugins.

## Development Conventions

- **State Management:** Uses React built-in hooks (`useState`, `useEffect`, `useCallback`).
- **Styling:** CSS is handled via `App.css` and `index.css`.
- **API Calls:** Fetches are performed in `useEffect` triggered by changes in search query, sort order, or page number.
- **Debouncing:** Search input is debounced to minimize API calls while typing.
- **Naming:** Follows standard React and JavaScript naming conventions (camelCase for variables/functions, PascalCase for components).
