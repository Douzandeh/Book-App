# 📚 Book App

A clean, responsive React application for browsing a curated collection of world literature classics. Search through timeless books, discover their origins, and save your favorites to a personal reading list — all in a sleek dark-themed interface.

**Live Demo:** [https://Douzandeh.github.io/Book-App](https://Douzandeh.github.io/Book-App)

---

## ✨ Features

- **Book Library** — Browse 10 of the world's most celebrated literary works, spanning from 1700 BCE to the 20th century
- **Live Search** — Filter books instantly by title using the search bar
- **Favorites List** — Like any book to add it to a personal Favorites sidebar; unlike to remove it
- **Book Details** — Each card displays the book cover, title, author, language, and page count
- **Dark UI** — Carefully styled dark theme with a purple accent, optimized for readability
- **Responsive Layout** — Two-column layout with the main book list and a collapsible favorites panel
- **GitHub Pages Deployment** — Production-ready with automated `gh-pages` deployment

---

## 🛠️ Technologies Used

| Category | Technology |
|---|---|
| Framework | [React 19](https://react.dev/) |
| Build Tool | [Vite 8](https://vitejs.dev/) with Rolldown bundler |
| Styling | CSS Modules |
| Icons | [react-icons 5](https://react-icons.github.io/react-icons/) |
| Linting | ESLint 10 with React Hooks plugin |
| Deployment | [gh-pages](https://www.npmjs.com/package/gh-pages) → GitHub Pages |

---

## 📸 Screenshots

> _Screenshots coming soon. Clone the project and run it locally to see it in action!_

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v20.19.0 or higher
- npm (comes with Node.js)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/Douzandeh/Book-App.git
   cd Book-App
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Start the development server**

   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173`

### Building for Production

```bash
npm run build
```

The production-ready files will be output to the `dist/` folder.

### Deploying to GitHub Pages

```bash
npm run deploy
```

This runs `vite build` then pushes the `dist/` folder to the `gh-pages` branch automatically.

---

## 📖 Usage

1. **Browse Books** — The full book list is shown on the main page on load
2. **Search** — Type a title (or partial title) into the search bar and click the search button to filter results. Clear the field and search again to reset
3. **Like a Book** — Click the ❤️ heart icon on any book card to add it to your Favorites panel on the right
4. **Unlike a Book** — Click the heart icon again to remove it from Favorites
5. **Visit Wikipedia** — _(coming soon — links are stored in the data)_

---

### Key Files

| File | Purpose |
|---|---|
| `src/constants/mockData.js` | Defines the 10 classic books with metadata and imported cover images |
| `src/components/Books.jsx` | Manages `books`, `liked`, and `search` state; orchestrates search filtering and favorites logic |
| `src/components/BookCard.jsx` | Renders a single book row with a toggle-able heart button using local `like` state |
| `src/layout/Layout.jsx` | Wraps the whole app in a consistent header (title + author link) and footer |

---

## 🔮 Future Improvements

- [ ] **Click-through to Wikipedia** — Make book titles/cards open their Wikipedia page in a new tab using the `link` field already present in the data
- [ ] **Pagination or infinite scroll** — Support larger book collections without overwhelming the page
- [ ] **Persistent favorites** — Save liked books to `localStorage` so favorites survive a page refresh
- [ ] **Filter by language or country** — Add dropdown filters alongside the title search
- [ ] **Sort options** — Sort by year, pages, or title alphabetically
- [ ] **Expanded book data** — Add genre, description, and rating fields
- [ ] **Responsive mobile layout** — Collapse the favorites panel into a bottom sheet or modal on small screens
- [ ] **Animations** — Smooth card entrance and heart-button micro-interactions
- [ ] **Real API integration** — Replace mock data with a live books API (e.g. Open Library)

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. **Fork** the repository
2. **Create** your feature branch: `git checkout -b feature/my-feature`
3. **Commit** your changes: `git commit -m 'Add some feature'`
4. **Push** to the branch: `git push origin feature/my-feature`
5. **Open a Pull Request** against `main`

Please make sure your code follows the existing ESLint configuration before submitting.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](./LICENSE) file for details.

---

<div align="center">
  <p>Developed with ❤️ by <a href="https://github.com/Douzandeh">Hossein Douzandeh</a></p>
</div>
