# Movie Explorer

A React-based web application that allows users to explore movies using the TMDB API. It features search, sorting, and pagination.

## Features

- **Search:** Search for movies with debouncing (500ms) to minimize API calls.
- **Sorting:** Sort movies by popularity, release date, and rating.
- **Pagination:** Browse through multiple pages of results.
- **Responsive Design:** A movie grid layout that adapts to different screen sizes.

## Tech Stack

- **Frontend:** React 19, Vite 8
- **Package Manager:** pnpm
- **API:** [The Movie Database (TMDB) API](https://www.themoviedb.org/documentation/api)

## Getting Started

### Prerequisites

- [pnpm](https://pnpm.io/installation) installed on your machine.
- A TMDB API Key.

### Installation

1. Clone the repository.
2. Navigate to the project directory:
   ```bash
   cd movie-explorer
   ```
3. Install dependencies:
   ```bash
   pnpm install
   ```
4. Create a `.env` file in the `movie-explorer` directory and add your TMDB API Key:
   ```env
   VITE_TMDB_API_KEY=your_api_key_here
   ```

### Development

To start the development server:
```bash
pnpm dev
```

### Production

To build the project for production:
```bash
pnpm build
```

To preview the production build locally:
```bash
pnpm preview
```

## Linting

To run ESLint:
```bash
pnpm lint
```

## Deployment

The project is configured with a base path of `/CS349-H3/` for deployment (e.g., to GitHub Pages). A GitHub Actions workflow for deployment is included in `.github/workflows/deploy.yml`.
