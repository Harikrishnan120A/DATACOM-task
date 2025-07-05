# React Leaflet Bug Demonstration App

A React application built with Vite that demonstrates common bugs found in React applications using mapping libraries. This project is designed for educational purposes to help developers identify, debug, and fix common issues in JavaScript/React applications.

## 🚀 Technologies Used

- **React 18+** - Modern React with Hooks
- **Vite** - Fast build tool and development server
- **Leaflet** - Open-source mapping library
- **React-Leaflet** - React components for Leaflet maps
- **JavaScript (ES6+)** - Modern JavaScript features

## 🐛 Intentional Bugs Included

This application contains **70+ intentional bugs** across different categories:

### State Management Issues (Bugs 1-6)
- Missing dependencies in useEffect
- Potential state updates on unmounted components
- Not checking for duplicates
- Missing state cleanup

### Map Rendering Problems (Bugs 7-20)
- Missing Leaflet icon configuration
- useEffect without proper cleanup
- Creating objects in render causing re-renders
- Missing error boundaries around map components

### Form Validation Issues (Bugs 21-38)
- No input validation
- Missing error handling for parseFloat
- Not sanitizing input values
- Missing accessibility attributes

### API Integration Bugs (Bugs 39-56)
- Missing API keys
- No abort controllers for cleanup
- Generic error handling
- No rate limiting

### CSS/Styling Issues (Bugs 57-70)
- No responsive layout
- Missing focus styles for accessibility
- No loading animations
- Missing media queries

## 🔧 Setup Instructions

### Prerequisites
- Node.js (version 14 or higher)
- npm or yarn package manager

### Installation
1. Clone or download this repository
2. Open the project in VS Code
3. Install dependencies:
   ```bash
   npm install
   ```

### Running the Application
1. Start the development server:
   ```bash
   npm run dev
   ```
2. Open your browser and navigate to `http://localhost:5173`
3. Open browser developer tools to observe bugs and errors

## 🔍 How to Use This for Bug Identification

### 1. Initial Setup
- Run the application
- Open browser developer tools (F12)
- Check the Console tab for JavaScript errors
- Monitor the Network tab for failed requests

### 2. Common Issues to Look For

**Console Errors:**
- React warnings about missing dependencies
- Leaflet icon issues
- State update warnings

**UI Issues:**
- Map not displaying properly
- Form validation problems
- Missing error states

**Performance Issues:**
- Unnecessary re-renders
- Memory leaks
- Infinite loops

### 3. Testing Scenarios

**Map Functionality:**
- Try adding locations using the form
- Click on map markers
- Use the quick-add buttons
- Clear all locations

**Form Testing:**
- Submit empty forms
- Enter invalid coordinates
- Test rapid submissions

**Weather Widget:**
- Select different locations
- Observe API call failures
- Test refresh functionality

## 🛠️ Debugging Tools

### Browser Developer Tools
- **Console**: View JavaScript errors and warnings
- **Network**: Monitor API requests and failures
- **Elements**: Inspect DOM and CSS issues
- **Sources**: Set breakpoints for debugging
- **Performance**: Analyze performance issues

### React Developer Tools (Recommended Extension)
- Install React Developer Tools browser extension
- Monitor component state and props
- Track unnecessary re-renders
- Profile component performance

## 📝 Bug Categories Explanation

### State Management
React state management bugs often involve:
- Missing dependencies in useEffect hooks
- State updates on unmounted components
- Race conditions in async operations

### Memory Leaks
Common sources of memory leaks:
- Event listeners not cleaned up
- Intervals/timeouts not cleared
- Map instances not properly destroyed

### CSS Issues
Styling problems include:
- Missing responsive design
- Accessibility issues
- Performance impacts from CSS

## 🎯 Learning Objectives

After working with this application, you should be able to:
- Identify common React anti-patterns
- Use browser developer tools effectively
- Implement proper error handling
- Apply React best practices
- Debug mapping library issues

## 🔗 Additional Resources

- [React Documentation](https://react.dev/)
- [Leaflet Documentation](https://leafletjs.com/)
- [Chrome DevTools Documentation](https://developer.chrome.com/docs/devtools/)
- [React Developer Tools](https://react.dev/learn/react-developer-tools)

## 📦 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint (if configured)

## ⚠️ Important Notes

- This application contains intentional bugs for educational purposes
- Do not use this code as a template for production applications
- Some features (like weather API) may not work due to missing API keys
- The focus is on identifying and fixing bugs, not on functionality

---

**Remember**: The goal is to learn how to identify, debug, and fix common issues in React applications. Use this as a practice environment to improve your debugging skills!+ Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
