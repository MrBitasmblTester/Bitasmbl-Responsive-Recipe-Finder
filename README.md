# Bitasmbl-Responsive-Recipe-Finder

Responsive Recipe Finder is a beginner-friendly Vue.js and Tailwind CSS project that allows users to search for recipes and view dynamic recipe cards displaying images, ingredients, and cooking steps. The app emphasizes modular component structure, responsive design, and seamless API data rendering.

## Tech Stack

- Vue.js (v3)
- Tailwind CSS
- JavaScript (ES6+)
- Vite (dev server & build tool)

## Requirements

- Use functional React components and hooks
- Fetch data from a public API and render dynamically
- Implement mobile-responsive design using Tailwind CSS

## Installation

1. Clone the repository:
   bash
   git clone https://github.com/YourUsername/Bitasmbl-Responsive-Recipe-Finder.git
   
2. Navigate into the project directory:
   bash
   cd Bitasmbl-Responsive-Recipe-Finder
   
3. Install dependencies:
   bash
   npm install
   # or
   yarn install
   
4. Create a `.env` file at the root to store your API configuration:
   bash
   VITE_API_BASE_URL=https://api.example.com
   VITE_API_KEY=your_api_key_here
   

## Usage

1. Start the development server:
   bash
   npm run dev
   # or
   yarn dev
   
2. Open your browser and visit `http://localhost:3000`.
3. Use the search input to look up recipes, and view resulting cards with images, ingredients, and step-by-step instructions.

## Implementation Steps

1. **Scaffold Project** – Initialize a new Vue 3 project using Vite.
2. **Install Tailwind CSS** – Configure Tailwind via PostCSS and add base, components, and utilities.
3. **Create Components**:
   - `SearchBar.vue` for capturing user queries.
   - `RecipeCard.vue` for displaying individual recipe details.
   - `RecipeList.vue` to render a grid of `RecipeCard` components.
4. **Setup API Service** – Create a service module using `fetch` to request recipe data from the public API, handling loading and error states.
5. **State Management** – Use the Vue Composition API (reactive and ref) to manage search term, fetched data, and UI states.
6. **Responsive Layout** – Apply Tailwind utility classes to ensure the layout adapts to mobile, tablet, and desktop breakpoints.
7. **Render Data Dynamically** – Pass fetched recipe objects into `RecipeCard` props and iterate within `RecipeList`.
8. **Testing & Optimization** – Test on multiple screen sizes, optimize images, and fine-tune Tailwind configurations for production.
9. **Build & Deploy** – Run `npm run build` (or `yarn build`) and deploy the `dist` folder to your hosting provider.