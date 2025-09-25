# Todo App - Frontend Engineer Interview Exercise

## Overview
Build a complete todo application using React that persists data in localStorage. This exercise will demonstrate your skills in React development, state management, local storage handling, and creating a polished user interface.

## Requirements

### Core Functionality
1. **Add Todos**: Users can add new todo items
2. **View Todos**: Display all todos in a clean, organized list
3. **Toggle Completion**: Mark todos as completed/incomplete
4. **Delete Todos**: Remove todos from the list
5. **Edit Todos**: Edit existing todo text inline
6. **Persist Data**: All todos should persist in localStorage between sessions

### Technical Requirements
- Use React 18+ with TypeScript
- Use TailwindCSS for styling (no other CSS frameworks)
- Implement state management using React Context API
- Create a custom `useLocalStorage` hook for localStorage operations
- Use localStorage for data persistence
- Include proper error handling
- Write clean, maintainable code with good component structure
- Responsive design that works on mobile and desktop

### User Interface Requirements
- Clean, modern design
- Intuitive user experience
- Visual feedback for user actions

### Data Structure
Each todo should have at minimum:
```typescript
type Todo = {
  id: string;
  text: string;
  completed: boolean;
  createdAt: Date;
  updatedAt: Date;
}
```

### Key Features to Implement

1. **React Context**
   - Create a TodoContext to manage global todo state
   - Implement TodoProvider component to wrap the app
   - Use useContext hook in components to access todo state and actions

2. **Custom Hooks**
   - **Required**: Create a `useLocalStorage` hook for localStorage operations
   - Create a `useTodos` hook that manages all todo operations
   - Ensure proper error handling in hooks

3. **State Management**
   - Use React Context API for global state management
   - Manage loading states and error states
   - Handle edge cases (empty todos, localStorage failures)

4. **TailwindCSS Styling**
   - Use TailwindCSS utility classes for all styling
   - Implement responsive design with Tailwind breakpoints
   - Create clean, modern UI with proper spacing and typography
   - Use Tailwind's color palette and design system

5. **LocalStorage Integration**
   - Implement proper serialization/deserialization in `useLocalStorage` hook
   - Handle localStorage quota exceeded errors
   - Graceful fallback when localStorage is unavailable

## Bonus Features (Optional)
- **Filtering**: Show all/active/completed todos
- **Bulk Actions**: Select all, delete completed
- **Search/Filter**: Search through todos
- **Dark Mode**: Theme toggle
- **Priority Levels**: High/medium/low priority


