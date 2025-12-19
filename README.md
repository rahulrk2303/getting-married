# Sruthi & Rahul Wedding Website

A modern, responsive, and aesthetic wedding website built with **React**, **TypeScript**, and **Tailwind CSS**.

## Features

- **Hero Section**: Full-screen background with a live countdown timer to the wedding date.
- **Our Story**: A dedicated section introducing the bride and groom.
- **Event Details**: Schedule of events including Engagement, Wedding, and Receptions.
- **Gallery**: Interactive image carousel.
- **Locations**: Integrated Google Maps embeds for venue locations.
- **RSVP System**: Functional form to collect guest responses (stores data locally for demo purposes).
- **Contact**: Contact information and inquiry form.

## Tech Stack

- **React 19**: UI Library.
- **TypeScript**: Type safety.
- **Tailwind CSS**: Styling (loaded via CDN).
- **Framer Motion**: Animations.
- **Lucide React**: Icons.
- **Vite**: Build tool and development server.

## How to Run Locally

You will need **Node.js** installed on your computer.

1.  Open your terminal in the project folder.
2.  Install the dependencies:
    ```bash
    npm install
    ```
3.  Start the development server:
    ```bash
    npm run dev
    ```
4.  Open the URL shown in your terminal (usually `http://localhost:5173`).

## How to Deploy to GitHub Pages

1.  **Update `vite.config.ts`**: Ensure the `base` property is set to `'./'` (already configured).
2.  **Build the Project**:
    Run the following command in your terminal:
    ```bash
    npm run build
    ```
    This will create a `dist` folder containing the static files.

3.  **Upload to GitHub**:
    - Commit and push your code to your GitHub repository.

4.  **Deploy**:
    - **Option A (Manual)**:
        - Install the `gh-pages` package: `npm install gh-pages --save-dev`
        - Add a script to `package.json`: `"deploy": "gh-pages -d dist"`
        - Run `npm run deploy`.
    - **Option B (Settings)**:
        - Go to your Repository Settings > Pages.
        - Set the source to **GitHub Actions** (if using a workflow) or push the contents of your `dist` folder to a branch named `gh-pages` and select that branch here.

## Project Structure

- `index.html`: Main HTML file.
- `index.tsx`: Application entry point.
- `App.tsx`: Main application component.
- `components/`: UI components (Hero, Story, Gallery, etc.).
- `services/`: API simulation logic.
- `types.ts`: TypeScript interfaces.

## Customization

To change the wedding date:
1.  Open `components/Hero.tsx`.
2.  Update the `targetDate` variable in the `useEffect` hook.
3.  Update the display text in the JSX.
