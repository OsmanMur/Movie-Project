# Movie Explorer

A React movie browsing application built with Vite and The Movie Database (TMDB) API. Browse popular movies, search by title, and keep a personal favorites list in your browser.

## Features

- Popular movies loaded from TMDB.
- Search form for finding movies by title.
- Reusable movie cards.
- Add and remove favorites through shared React Context.
- Favorites stored in localStorage.
- Separate home and favorites views with React Router.

## Technologies

React 18, JavaScript, Vite 6, React Router, CSS, and the Fetch API.

## Run Locally

Requires Node.js and npm compatible with Vite 6.

```bash
git clone https://github.com/OsmanMur/Movie-Project.git
cd Movie-Project
npm ci
npm run dev
```

Open the local URL printed by Vite.

The API configuration is in `src/services/api.js`. The current implementation reads an `API_KEY` constant there; movie requests require a valid TMDB API key. Browser-side API credentials are visible to visitors.

## Other Commands

```bash
npm run build
npm run preview
npm run lint
```

The build creates the production assets; preview serves that build locally.

## Code Guide

| Path | Responsibility |
| --- | --- |
| `src/pages/Home.jsx` | Popular movie loading, search, and result display |
| `src/pages/Favorites.jsx` | Saved movie view |
| `src/components/MovieCard.jsx` | Individual movie card |
| `src/components/NavBar.jsx` | Navigation |
| `src/context/MovieContext.jsx` | Shared favorites state and browser persistence |
| `src/services/api.js` | TMDB requests |
| `src/css/` | Application styles |

## Learning Focus

Working with API requests, React state and effects, reusable components, client-side routing, and shared application state.

## Data Source

Movie data and images are provided by [The Movie Database](https://www.themoviedb.org/). This application is not endorsed or certified by TMDB.
