# Splash App - Next.js Project Setup

## Overview
Splash App is a modern web application built with Next.js, TypeScript, and Tailwind CSS. The project demonstrates best practices in React development, including shared layouts, component reusability, and proper TypeScript interface management.

## 🚀 Features
- Shared layout implementation with header and footer
- Custom reusable button component
- Google Fonts integration (Montserrat)
- TypeScript interfaces for type safety
- Imperative routing using Next.js router
- Custom 404 error page
- Responsive design with Tailwind CSS
- Social media integration in footer

## 🛠 Tech Stack
- Next.js
- TypeScript
- Tailwind CSS
- React Icons
- Google Fonts (Montserrat)

## 📦 Project Structure
```
alx-project-0x03/
├── components/
│   ├── common/
│   │   └── Button.tsx
│   └── layouts/
│       ├── Header.tsx
│       ├── Footer.tsx
│       └── Layout.tsx
├── interface/
│   └── index.ts
├── pages/
│   ├── _app.tsx
│   ├── index.tsx
│   └── 404.tsx
└── styles/
    └── global.css
```

## 🚀 Getting Started

### Prerequisites
- Node.js (version 14 or higher)
- npm

### Installation
1. Clone the repository
```bash
git clone https://github.com/Dayvid0063/alx-project-0x03-setup.git
cd alx-project-0x03
```

2. Install dependencies
```bash
npm install
```

3. Run the development server
```bash
npm run dev
```

4. Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## 🎯 Key Features Explained

### Shared Layout
The project implements a shared layout pattern using the Layout component, which includes:
- Header with navigation and authentication buttons
- Footer with social media links and site information
- Consistent styling across all pages

### Custom Button Component
A reusable button component with:
- Customizable colors (red, blue, orange, green)
- Configurable sizes
- Click action handlers
- TypeScript type safety

### Interface Management
All TypeScript interfaces are centralized in the `interface/index.ts` file for better maintainability:
- ButtonProps
- LayoutProps
- PageRouteProps

### Custom 404 Page
A user-friendly 404 error page featuring:
- Gradient background
- Engaging error message
- Home navigation button
- Responsive design

### Google Fonts Integration
The project uses the Montserrat font family:
- Applied globally through CSS
- Includes all weights and styles
- Optimized loading

## 📝 Component Usage Examples

### Button Component
```typescript
<Button
  buttonLabel="Sign In"
  buttonBackgroundColor="red"
  action={() => handleSignIn()}
/>
```

### Layout Component
```typescript
<Layout>
  <YourPageContent />
</Layout>
```

## 🔄 Routing
The application uses Next.js's file-based routing system with imperative navigation:
```typescript
const routeToNextPage = ({ pageRoute }: PageRouteProps) => {
  router.push(pageRoute, undefined, { shallow: false})
}
```

## 🎨 Styling
- Utilizes Tailwind CSS for responsive design
- Custom color schemes for different components
- Consistent spacing and typography

## 📱 Responsive Design
- Mobile-first approach
- Responsive navigation
- Flexible grid layouts
- Adaptive typography

## 🔧 Development Practices
- Type safety with TypeScript
- Component reusability
- DRY (Don't Repeat Yourself) principles
- Clean code organization
