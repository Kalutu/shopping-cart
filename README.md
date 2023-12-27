# Shopping Cart App
This is a shopping cart application built using React, Redux Toolkit, and asynchronous data fetching with `createAsyncThunk`. The app allows users to add products to their cart, update quantities, view a summary of selected items, and clear the entire cart. It also features a modal for confirming the clearing of the cart.

## Components
### 1. `CartContainer`

- **Description:** Displays the user's shopping cart with the list of items, their quantities, and a total price.
- **File:** `src/components/CartContainer.js`

### 2. `CartItem`
- **Description:** Represents an individual item in the shopping cart with options to increase, decrease, or remove the item.
- **File:** `src/components/CartItem.js`

### 3. `Modal`
- **Description:** A modal component that prompts the user to confirm clearing the entire shopping cart.
- **File:** `src/components/Modal.js`

### 4. `Navbar`
- **Description:** Displays a navigation bar at the top of the app, showing the app name and the total number of items in the cart.
- **File:** `src/components/Navbar.js`

## Features
- **Adding Items:** Users can add products to the cart.
- **Removing Items:** Users can remove individual items from the cart.
- **Updating Quantities:** Users can increase or decrease the quantity of items in the cart.
- **Clearing Cart:** Users can clear the entire cart with a confirmation modal.
- **Asynchronous Data Fetching:** Product data is fetched asynchronously from the "https://course-api.com/react-useReducer-cart-project" API using `createAsyncThunk`.

## Installation

1. Clone the repository:  ``` git clone https://github.com/Kalutu/shopping-cart```
2. Change into the project directory: `cd shopping-cart`
3. Install dependencies: ``` npm install ```
4. Start the development server: ``` npm start ```
The app will be accessible at http://localhost:3000 by default.

## Usage
1. Browse the list of available products.
2. Click on a product to view details and add it to the cart.
3. Navigate to the cart to view and update selected items.
4. Adjust quantities or remove items as needed.
5. Clear the entire cart using the "Clear Cart" button with a confirmation modal.

## Folder Structure
- **src/components:** Contains React components.
- **src/features/cart:** Redux Toolkit slice for managing the cart state.
- **src/features/modal:** Redux Toolkit slice for managing the modal state.

## Redux State Management
**Cart State:**
- `cartItems`: An array containing the selected items in the cart.
- `amount`: The total quantity of items in the cart.
- `total`: The total price of all items in the cart.
- `isLoading`: Indicates whether data is still being fetched.

**Modal State:**
- `isOpen`: Indicates whether the modal is open.

## Contributing
We welcome contributions! If you find a bug or have a feature request, please open an issue or submit a pull request.
