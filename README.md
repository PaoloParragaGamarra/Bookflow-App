# BookFlow Frontend

![Angular](https://img.shields.io/badge/Angular-17.3.6-red?logo=angular)
![TypeScript](https://img.shields.io/badge/TypeScript-5.4.2-blue?logo=typescript)
![Firebase](https://img.shields.io/badge/Firebase-Hosting-orange?logo=firebase)
![Material UI](https://img.shields.io/badge/Angular%20Material-17.3.6-purple?logo=material-ui)

BookFlow is an Angular-based frontend web application for book management, reading clubs, and book recommendations among users.

## ✨ Features

- 📚 **Book Management**: Explore, search, and view book details
- 👥 **Reading Clubs**: Create and join reading clubs
- 💬 **Comment System**: Comment and discuss books
- 🔍 **Recommendations**: Recommendation system between friends
- 📊 **Personal Lists**: Create reading lists and favorite authors
- 👤 **Profile Management**: Edit profile and manage subscriptions
- 💳 **Payment System**: Premium subscription management
- 📱 **Responsive Design**: Interface adapted to different devices

## 🛠️ Technologies Used

- **Framework**: Angular 17.3.6
- **UI Library**: Angular Material 17.3.6
- **Language**: TypeScript 5.4.2
- **Styling**: CSS3 with Material Design
- **HTTP Client**: Angular HttpClient with RxJS
- **Routing**: Angular Router
- **Build Tool**: Angular CLI
- **Backend Mock**: JSON Server
- **Hosting**: Firebase Hosting
- **Testing**: Jasmine & Karma

## 📁 Project Structure

```
src/
├── app/
│   ├── bookflow/                    # Main application module
│   │   ├── components/              # Application components
│   │   │   ├── book-card/           # Book card
│   │   │   ├── book-comment/        # Book comments
│   │   │   ├── book-detail/         # Book details
│   │   │   ├── book-home/           # Home page
│   │   │   ├── book-profile/        # User profile
│   │   │   ├── book-reading-club/   # Reading clubs
│   │   │   ├── book-recommend/      # Recommendations
│   │   │   ├── book-listas/         # Personal lists
│   │   │   ├── book-subscription/   # Subscriptions
│   │   │   └── payment-details/     # Payment details
│   │   ├── model/                   # Data models
│   │   └── services/                # Application services
│   ├── public/                      # Public components
│   │   └── components/
│   │       ├── header/              # Header
│   │       └── footer/              # Footer
│   ├── app.component.*              # Root component
│   ├── app.config.ts                # App configuration
│   └── app.routes.ts                # Routes configuration
├── assets/                          # Static resources
├── environments/                    # Environment variables
└── styles.css                       # Global styles
```

## 🚀 Installation and Setup

### Prerequisites

- Node.js (version 18 or higher)
- npm (version 9 or higher)
- Angular CLI (version 17.3.6)

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd FRONT_END2
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure mock server** (optional)
   ```bash
   # JSON server is configured in server/db.json
   npx json-server --watch server/db.json --routes server/routes.json --port 3000
   ```

## 🔧 Available Scripts

| Script | Description |
|--------|--------------|
| `npm start` | Starts development server at `http://localhost:4200` |
| `npm run build` | Builds the app for production |
| `npm run watch` | Builds the app in watch mode |
| `npm test` | Runs unit tests |
| `ng serve` | Angular development server |
| `ng build` | Build for production |
| `ng test` | Unit tests with Karma |

## 🌐 Development

### Development Server

```bash
npm start
# or
ng serve
```

Navigate to `http://localhost:4200/`. The application will automatically reload if you make changes to the source files.

### Generate Components

```bash
# Generate a new component
ng generate component component-name

# Other available schematics
ng generate directive|pipe|service|class|guard|interface|enum|module
```

### Production Build

```bash
npm run build
# or
ng build
```

The build artifacts will be stored in the `dist/` directory.

## 🧪 Testing

### Unit Tests

```bash
npm test
# or
ng test
```

Runs unit tests via [Karma](https://karma-runner.github.io).

### Code Coverage

```bash
ng test --code-coverage
```

## 🚀 Deployment

### Firebase Hosting

The application is configured for Firebase Hosting deployment:

```bash
# Install Firebase CLI
npm install -g firebase-tools

# Firebase login
firebase login

# Deploy
firebase deploy
```

### Firebase Configuration

- **Hosting**: Configured in `firebase.json`
- **Emulators**: Port 5000 for local development
- **Public Directory**: `dist/frontend-bookflow-test/browser`

## 📱 Main Features

### 🏠 Home Page
- Dashboard with trending books
- Main navigation
- Quick access to features

### 📚 Book Management
- **Explore books**: Complete catalog with filters
- **Book details**: Complete information, comments and reviews
- **Personal lists**: Create and manage reading lists

### 👥 Reading Clubs
- **Create clubs**: Form new reading groups
- **Join clubs**: Participate in existing clubs
- **Management**: Manage members and activities

### 💬 Social System
- **Comments**: Comment and rate books
- **Recommendations**: Recommend books to friends
- **Profiles**: Manage personal profile

### 💳 Subscriptions
- **Premium plans**: Access to advanced features
- **Payment management**: Process payments and subscriptions
- **History**: Track transactions

## 🎨 Themes and Styling

- **Material Design**: Implemented with Angular Material
- **Theme**: Default Indigo-Pink
- **Responsive**: Adapted for mobile, tablet, and desktop
- **Custom CSS**: Custom styles in `src/styles.css`

## 📊 API and Backend

- **Mock Server**: JSON Server for development (`server/db.json`)
- **API Routes**: Configured in `server/routes.json`
- **Base URL**: `/api/v1/*` mapped to server routes

## 🤝 Contributing

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Development Notes

### Useful Commands

```bash
# Linting
ng lint

# Bundle analysis
ng build --stats-json
npx webpack-bundle-analyzer dist/frontend-bookflow-test/stats.json

# Update dependencies
ng upda