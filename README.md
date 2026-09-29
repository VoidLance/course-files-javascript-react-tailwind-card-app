# React + Tailwind CSS Card App

A small card-management interface built with React, Vite, and Tailwind CSS. The app demonstrates how to render reusable card components from state, add cards through a form, and switch between light and dark themes.

## Features

- Displays cards with an image, title, description, and action label.
- Adds new cards from the form without reloading the page.
- Toggles Tailwind CSS dark mode using the `dark` class strategy.
- Uses responsive utility classes to lay out cards in a flexible grid.

## Tech stack

- [React](https://react.dev/) for the user interface
- [Vite](https://vite.dev/) for development and production builds
- [Tailwind CSS](https://tailwindcss.com/) for styling
- [ESLint](https://eslint.org/) for code quality checks

## Getting started

### Prerequisites

- [Node.js](https://nodejs.org/) 18 or newer
- npm (included with Node.js)

### Installation

1. Clone the repository and open the project directory.
2. Install the dependencies:

   ```bash
   npm install
   ```

### Development

Start the Vite development server:

```bash
npm run dev
```

Open the local URL shown in the terminal, usually `http://localhost:5173`.

### Production build

Create an optimized production build:

```bash
npm run build
```

Preview the production build locally:

```bash
npm run preview
```

### Linting

Run ESLint across the project:

```bash
npm run lint
```

## Project structure

```text
.
├── src/
│   ├── components/
│   │   └── Card.jsx       # Reusable card component
│   ├── App.jsx            # Card state, form, and theme toggle
│   ├── App.css            # App-level styles
│   ├── index.css          # Tailwind directives and global styles
│   └── main.jsx           # React application entry point
├── tailwind.config.js     # Tailwind content and dark-mode configuration
├── postcss.config.cjs     # PostCSS configuration
└── package.json           # Scripts and dependencies
```

## How it works

The initial cards are defined in `src/App.jsx`. The form stores its input in local React state and appends a new card to the collection when submitted. `src/components/Card.jsx` receives each card's data as props and renders the card UI.

The theme toggle adds or removes the `dark` class on the app's root container. Tailwind's `dark:` variants then apply the dark theme styles.

## License

This project is intended for learning and experimentation. No license has been specified.
