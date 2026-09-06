# Multi-Vendor Mobile Shopping App

A modern, cross-platform mobile shopping application built with React Native and Expo, designed to provide a seamless shopping experience across multiple vendors.

## 🚀 Features

### Core Features
- **Multi-Vendor Support**: Browse and shop from multiple vendors in one app
- **Product Catalog**: Comprehensive product browsing with categories and filters
- **Favorites System**: Save and manage favorite products
- **Search & Filter**: Advanced search and filtering capabilities
- **User Authentication**: Secure login and user management
- **Responsive Design**: Optimized for both mobile and tablet devices

### User Experience
- **Modern UI/UX**: Clean, intuitive interface with smooth animations
- **Dark/Light Theme**: Automatic theme switching based on system preferences
- **Offline Support**: Basic offline functionality with local storage
- **Haptic Feedback**: Enhanced user interaction with haptic responses
- **Image Optimization**: Fast loading images with blur placeholders

### Technical Features
- **TypeScript**: Full type safety throughout the application
- **State Management**: Efficient state management with Zustand
- **Data Fetching**: Optimized data fetching with React Query
- **Navigation**: Seamless navigation with Expo Router
- **Performance**: Optimized for smooth performance on all devices

## 🛠 Tech Stack

### Frontend
- **React Native** (0.79.1) - Cross-platform mobile development
- **Expo** (53.0.4) - Development platform and tools
- **TypeScript** (5.8.3) - Type safety and better development experience
- **NativeWind** (4.1.23) - Tailwind CSS for React Native

### State Management & Data
- **Zustand** (5.0.2) - Lightweight state management
- **React Query** (5.83.0) - Server state management and caching
- **AsyncStorage** (2.1.2) - Local data persistence

### Navigation & UI
- **Expo Router** (5.0.3) - File-based routing
- **React Navigation** (7.1.6) - Navigation library
- **Lucide React Native** (0.475.0) - Beautiful icons
- **Expo Image** (2.1.6) - Optimized image component

### Development Tools
- **ESLint** (9.31.0) - Code linting
- **Expo CLI** - Development and build tools

## 📱 Screenshots

*Screenshots will be added here*

## 🚀 Getting Started

### Prerequisites

- **Node.js** (v18 or higher)
- **npm** or **yarn**
- **Expo CLI** (`npm install -g @expo/cli`)
- **iOS Simulator** (for iOS development) or **Android Studio** (for Android development)

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd multi-vendor-shopping-app-new
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Start the development server**
   ```bash
   npm start
   # or
   yarn start
   ```

4. **Run on your preferred platform**
   ```bash
   # iOS
   npm run ios
   
   # Android
   npm run android
   
   # Web
   npm run web
   ```

## 📁 Project Structure

```
multi-vendor-shopping-app-new/
├── app/                    # Expo Router app directory
│   ├── (tabs)/            # Tab-based navigation
│   │   ├── index.tsx      # Home screen
│   │   ├── browse.tsx     # Product browsing
│   │   ├── favorites.tsx  # Favorites screen
│   │   └── settings.tsx   # Settings screen
│   ├── login.tsx          # Authentication screen
│   └── product/           # Product detail screens
│       └── [id].tsx       # Dynamic product routes
├── components/            # Reusable UI components
│   ├── ProductCard.tsx    # Product display component
│   ├── SearchBar.tsx      # Search functionality
│   ├── FilterChips.tsx    # Filter components
│   └── LoadingSpinner.tsx # Loading states
├── hooks/                 # Custom React hooks
│   ├── useAuth.tsx        # Authentication logic
│   ├── useProducts.tsx    # Product data management
│   ├── useFavorites.tsx   # Favorites functionality
│   └── useVendor.tsx      # Vendor data management
├── services/              # API and storage services
│   ├── api.ts            # API client and endpoints
│   └── storage.ts        # Local storage utilities
├── types/                 # TypeScript type definitions
│   ├── product.ts        # Product-related types
│   ├── user.ts           # User-related types
│   └── vendor.ts         # Vendor-related types
└── assets/               # Static assets
    └── images/           # App icons and images
```

## 🔧 Configuration

### Environment Variables

Create a `.env` file in the root directory:

```env
# API Configuration
API_BASE_URL=your_api_base_url
API_KEY=your_api_key

# App Configuration
APP_NAME=Multi-Vendor Shopping App
APP_VERSION=1.0.0
```

### App Configuration

The app configuration is managed in `app.json`:

```json
{
  "expo": {
    "name": "Multi-Vendor Mobile Shopping App",
    "slug": "multi-vendor-mobile-shopping-app",
    "version": "1.0.0",
    "orientation": "portrait",
    "userInterfaceStyle": "automatic"
  }
}
```

## 📱 Available Scripts

- `npm start` - Start the Expo development server
- `npm run android` - Run on Android device/emulator
- `npm run ios` - Run on iOS device/simulator
- `npm run web` - Run in web browser
- `npm run lint` - Run ESLint for code quality

## 🏗 Architecture

### State Management
The app uses **Zustand** for global state management and **React Query** for server state:

- **Zustand**: Manages user authentication, favorites, and app preferences
- **React Query**: Handles API data fetching, caching, and synchronization

### Data Flow
1. **API Layer**: Centralized API client in `services/api.ts`
2. **Custom Hooks**: Business logic encapsulated in custom hooks
3. **Components**: UI components consume data through hooks
4. **Local Storage**: Persistent data stored using AsyncStorage

### Navigation
- **Expo Router**: File-based routing system
- **Tab Navigation**: Main app sections (Home, Browse, Favorites, Settings)
- **Stack Navigation**: Product details and authentication flows

## 🎨 UI/UX Design

### Design System
- **Typography**: Consistent text hierarchy and spacing
- **Colors**: Dynamic theming with vendor-specific primary colors
- **Components**: Reusable, accessible UI components
- **Animations**: Smooth transitions and micro-interactions

### Accessibility
- **Screen Reader Support**: Proper accessibility labels
- **Color Contrast**: WCAG compliant color combinations
- **Touch Targets**: Adequate touch target sizes
- **Keyboard Navigation**: Full keyboard accessibility

## 🔒 Security

- **Authentication**: Secure user authentication flow
- **Data Validation**: Input validation and sanitization
- **API Security**: Secure API communication
- **Local Storage**: Encrypted sensitive data storage

## 🧪 Testing

### Running Tests
```bash
# Run all tests
npm test

# Run tests in watch mode
npm run test:watch

# Run tests with coverage
npm run test:coverage
```

### Testing Strategy
- **Unit Tests**: Individual component and hook testing
- **Integration Tests**: API and state management testing
- **E2E Tests**: Full user flow testing

## 📦 Building for Production

### Android
```bash
expo build:android
```

### iOS
```bash
expo build:ios
```

### Web
```bash
expo build:web
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines
- Follow TypeScript best practices
- Write meaningful commit messages
- Add tests for new features
- Update documentation as needed
- Follow the existing code style

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

If you encounter any issues or have questions:

1. Check the [Issues](../../issues) page for existing solutions
2. Create a new issue with detailed information
3. Contact the development team

## 🙏 Acknowledgments

- **Expo Team** for the amazing development platform
- **React Native Community** for the excellent ecosystem
- **All Contributors** who have helped improve this project

---

**Made with ❤️ using React Native and Expo**
