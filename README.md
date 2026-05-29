### Task Overview
You are building a core feature for an e-commerce startup’s proof-of-concept website—a simple, yet robust, Shopping Cart. Customers need to browse a catalog of products fetched asynchronously from an API, add products to their cart, and manage the cart’s contents in real-time. You are provided a project scaffold, product type definitions, and mock fetch utilities; your main challenge is to implement state management, asynchronous product loading, cart UI updates, and responsive performance. Good architecture is key to future scaling and smooth customer UX.

### Objectives
- Build a Products List that displays all products fetched from the API.
- Enable users to add items to the cart. If an item is already in the cart, increase its quantity accordingly.
- Display a Cart Sidebar reflecting current cart items, their quantities, and the total price. Users must be able to remove or change item quantities directly from the sidebar.
- Show a loading indicator when products are being fetched and handle any errors with a meaningful message.
- Ensure cart operations are instant, accurate, and do not cause unnecessary component re-renders.
- Use TypeScript for all files, leveraging type definitions provided.
- Maintain a project structure that separates concerns.

### How to Verify
- When you start the app, a loading indicator shows until products load, or an error message is displayed if the fetch fails.
- The catalog correctly lists all products. Adding an item increases its count in the cart and updates the total instantly in the sidebar.
- Quantity and remove actions in the sidebar immediately reflect in both the cart and total price. The UI does not flicker or lag.
- Cart logic does not duplicate items; adding the same product increases its quantity.
- Code is organized with a modular file and folder structure and uses proper TypeScript typing throughout.

### Helpful Tips
- Consider how state should flow through your component tree to avoid prop drilling or unnecessary complexity.
- Think about which components truly need to re-render when cart data changes.
- Explore React's built-in hooks for managing side effects that occur when the component first mounts.
- Review patterns for handling asynchronous operations and their various states.
- Consider how to structure data to make cart operations like quantity updates and item removal straightforward.
