# 🎮 Poke Front Angular

> Angular application consuming PokéAPI - Responsive Pokémon explorer with modern UI

**Author:** José Eduardo Tirado Verbel  
**Demo:** [View Live Demo](https://jotive.github.io/poke-front-angular)

## 📝 Overview

This is a modern Angular application that consumes the [PokéAPI](https://pokeapi.co/) to provide an interactive and responsive Pokémon explorer. Built with Angular and TypeScript, this project demonstrates proficiency in consuming RESTful APIs, component-based architecture, and responsive design principles.

## ✨ Features

- ✅ Browse and search Pokémon database
- ✅ View detailed Pokémon information (stats, abilities, types)
- ✅ Responsive design for all device sizes
- ✅ Modern and clean user interface
- ✅ Real-time API data fetching
- ✅ Efficient state management
- ✅ TypeScript for type safety
- ✅ Modular component architecture

## 🛠️ Tech Stack

- **Angular** - Frontend framework
- **TypeScript** - Programming language
- **RxJS** - Reactive programming
- **PokéAPI** - RESTful Pokémon API
- **HTML5/CSS3/Sass** - Markup and styling
- **Angular CLI** - Development tooling
- **Git** - Version control

## 📁 Project Structure

```
poke-front-angular/
├── poke-api-front/
│   ├── src/
│   │   ├── app/
│   │   │   ├── components/     # UI components
│   │   │   ├── services/       # API services
│   │   │   ├── models/         # Data models
│   │   │   ├── pipes/          # Custom pipes
│   │   │   └── app.module.ts   # Root module
│   │   ├── assets/            # Static assets
│   │   ├── styles.scss        # Global styles
│   │   └── index.html         # Entry point
│   ├── angular.json          # Angular config
│   ├── package.json          # Dependencies
│   └── tsconfig.json         # TypeScript config
└── README.md                # Documentation
```

## 🚀 Getting Started

### Prerequisites

- Node.js 14.x or higher
- npm 6.x or higher
- Angular CLI 12.x or higher

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/jotive/poke-front-angular.git
   cd poke-front-angular/poke-api-front
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   ng serve
   # or
   npm start
   ```

4. **Access the application:**
   - Navigate to `http://localhost:4200` in your browser
   - The app will automatically reload if you change any source files

## 📚 Key Features Implementation

### API Integration

The application uses Angular's `HttpClient` to consume the PokéAPI:

```typescript
// Example service call
getPokemon(id: number): Observable<Pokemon> {
  return this.http.get<Pokemon>(`https://pokeapi.co/api/v2/pokemon/${id}`);
}
```

### Component Architecture

- **PokemonListComponent** - Displays grid/list of Pokémon
- **PokemonDetailComponent** - Shows detailed Pokémon information
- **SearchComponent** - Handles Pokémon search functionality
- **HeaderComponent** - Navigation and branding

### Responsive Design

- Mobile-first approach
- Flexbox/Grid layouts
- Breakpoints for tablet and desktop views
- Touch-friendly interface

## 🔧 Build & Deployment

### Build for Production

```bash
ng build --prod
# Output will be in dist/ directory
```

### Deploy to GitHub Pages

```bash
ng build --prod --base-href /poke-front-angular/
npx angular-cli-ghpages --dir=dist/poke-api-front
```

## 🧪 Testing

### Run Unit Tests

```bash
ng test
# Run tests with code coverage
ng test --code-coverage
```

### Run End-to-End Tests

```bash
ng e2e
```

## 🎯 Project Goals Achieved

✅ Successfully consume external RESTful API  
✅ Implement responsive and modern UI  
✅ Component-based architecture  
✅ TypeScript best practices  
✅ Reactive programming with RxJS  
✅ Angular CLI for development workflow  
✅ Clean code and project structure  

## 📸 Screenshots

_Note: Add screenshots showing the Pokémon list, detail views, and responsive layouts_

## 🛣️ Roadmap & Future Enhancements

- [ ] Add Pokémon comparison feature
- [ ] Implement favorites/bookmarks functionality
- [ ] Add advanced search filters (type, generation, stats)
- [ ] Integrate Pokémon evolution chains
- [ ] Add unit and e2e test coverage
- [ ] Implement state management (NgRx/Akita)
- [ ] Add animations and transitions
- [ ] PWA capabilities (offline mode)
- [ ] Dark mode theme

## 📚 Resources

- [PokéAPI Documentation](https://pokeapi.co/docs/v2)
- [Angular Documentation](https://angular.io/docs)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/)
- [RxJS Documentation](https://rxjs.dev/guide/overview)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 📧 Contact

**José Eduardo Tirado Verbel**
- Portfolio: [jotive.com.co](https://jotive.com.co)
- GitHub: [@jotive](https://github.com/jotive)
- Email: jotive@gmail.com

---

⭐ If you found this project helpful, please consider giving it a star!  
🐞 Report bugs or suggest features by opening an issue.
