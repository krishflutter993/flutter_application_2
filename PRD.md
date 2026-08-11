# PRD: Food Delivery Flutter App

## 1. Project Overview

Build a modern, production-ready food delivery mobile application using Flutter.

The application should allow users to:

* Create an account and log in
* Browse restaurants
* Browse food categories
* Search for restaurants and food
* View food details
* Add food to cart
* Modify cart items
* Manage delivery address
* Select payment method
* Place orders
* View order history
* Track order status
* Manage profile and account settings

The application must have a clean, modern, responsive mobile UI.

---

# 2. Technical Requirements

## Technology

* Flutter
* Dart
* Material 3
* Responsive UI
* Clean and maintainable architecture
* Reusable widgets
* Proper error handling
* Loading states
* Empty states
* Form validation

## Architecture

Use a clean modular project structure.

Recommended structure:

```text
lib/
├── core/
├── models/
├── services/
├── repositories/
├── providers/
├── widgets/
├── screens/
│   ├── auth/
│   ├── home/
│   ├── restaurant/
│   ├── food/
│   ├── cart/
│   ├── checkout/
│   ├── orders/
│   └── profile/
├── utils/
└── main.dart
```

Use reusable components instead of duplicating UI code.

---

# 3. UI/UX Requirements

Create a modern food delivery design.

The application should include:

* Clean typography
* Rounded cards
* Food images
* Restaurant cards
* Category cards
* Modern buttons
* Bottom navigation
* Smooth navigation
* Loading indicators
* Error messages
* Empty states
* Responsive layouts

Do not use unnecessarily complicated animations.

The UI should work correctly on different mobile screen sizes.

---

# 4. Task 1: Project Setup

Create and configure the Flutter project.

Requirements:

* Verify Flutter project configuration
* Configure Material 3
* Configure application theme
* Configure light and dark theme support
* Create the base folder structure
* Add required dependencies only when needed
* Ensure the project builds successfully

Acceptance criteria:

* Flutter project runs successfully
* No compilation errors
* Folder structure is organized
* Material 3 is configured

---

# 5. Task 2: Application Theme

Create the global application theme.

Requirements:

* Primary color
* Secondary color
* Background color
* Surface colors
* Text styles
* Button styles
* Card styles
* Input field styles
* App bar styles

Create centralized theme configuration.

Acceptance criteria:

* All screens use the centralized theme
* No unnecessary hardcoded colors
* UI remains consistent throughout the application

---

# 6. Task 3: Navigation System

Create the main application navigation.

Requirements:

* Authentication navigation
* Main application navigation
* Bottom navigation
* Home
* Search
* Orders
* Profile

Acceptance criteria:

* Navigation works correctly
* Back navigation works correctly
* Authentication state determines the correct initial screen

---

# 7. Task 4: Splash Screen

Create a splash screen.

Requirements:

* Application logo
* Application name
* Loading indicator if necessary
* Check authentication state
* Navigate to Login if user is not authenticated
* Navigate to Home if user is authenticated

Acceptance criteria:

* Splash screen displays correctly
* Correct screen opens after initialization

---

# 8. Task 5: Registration

Create the registration screen.

Fields:

* Full name
* Email
* Phone number
* Password
* Confirm password

Requirements:

* Form validation
* Required field validation
* Email validation
* Password validation
* Password confirmation validation
* Loading state
* Error state
* Success handling

Acceptance criteria:

* Invalid data cannot be submitted
* Valid registration data can be submitted
* User receives useful error messages

---

# 9. Task 6: Login

Create the login screen.

Fields:

* Email
* Password

Features:

* Login button
* Forgot password
* Navigate to registration
* Loading state
* Error state

Acceptance criteria:

* Valid login works
* Invalid credentials show an error
* User is redirected to Home after successful login

---

# 10. Task 7: Forgot Password

Create forgot password functionality.

Requirements:

* Email input
* Validation
* Submit button
* Success message
* Error message

Acceptance criteria:

* Invalid email is rejected
* Valid email request is processed
* User receives clear feedback

---

# 11. Task 8: Home Screen

Create the main home screen.

Sections:

* Greeting
* User profile/avatar
* Search bar
* Promotional banner
* Food categories
* Popular restaurants
* Popular foods
* Recommended foods

Requirements:

* Scrollable layout
* Responsive cards
* Loading state
* Empty state
* Error state

Acceptance criteria:

* Home screen is visually polished
* All sections render correctly
* Navigation to restaurant and food details works

---

# 12. Task 9: Food Categories

Create food category functionality.

Example categories:

* Pizza
* Burger
* Indian
* Chinese
* Mexican
* Desserts
* Drinks
* Healthy

Requirements:

* Category cards
* Category icon/image
* Category name
* Category selection

Acceptance criteria:

* User can select a category
* Selected category filters the food/restaurant list

---

# 13. Task 10: Search

Create search functionality.

Requirements:

* Search bar
* Search restaurants
* Search foods
* Search results
* Empty search state
* No-results state
* Clear search button

Acceptance criteria:

* Search results update correctly
* Search can be cleared
* No-results state is displayed properly

---

# 14. Task 11: Restaurant Listing

Create restaurant listing screen.

Restaurant card should contain:

* Restaurant image
* Restaurant name
* Rating
* Delivery time
* Delivery fee
* Cuisine type
* Favorite button

Requirements:

* Restaurant list
* Loading state
* Empty state
* Error state

Acceptance criteria:

* Restaurants display correctly
* User can open restaurant details

---

# 15. Task 12: Restaurant Details

Create restaurant details screen.

Display:

* Restaurant image
* Restaurant name
* Rating
* Delivery time
* Address
* Cuisine
* Description
* Menu categories
* Food items

Acceptance criteria:

* Restaurant information displays correctly
* Food items are selectable
* User can open food details

---

# 16. Task 13: Food Details

Create food details screen.

Display:

* Food image
* Food name
* Description
* Price
* Rating
* Ingredients
* Available customization options
* Quantity selector

Features:

* Add to Cart
* Favorite

Acceptance criteria:

* User can change quantity
* User can customize food if options exist
* User can add item to cart

---

# 17. Task 14: Favorites

Create favorites functionality.

Requirements:

* Add/remove restaurant from favorites
* Add/remove food from favorites
* Favorites screen
* Empty favorites state

Acceptance criteria:

* Favorite state persists
* User can remove favorites
* Favorites display correctly

---

# 18. Task 15: Cart

Create shopping cart functionality.

Cart item should contain:

* Food image
* Food name
* Price
* Quantity
* Remove button

Cart should calculate:

* Subtotal
* Delivery fee
* Tax
* Discount
* Final total

Features:

* Increase quantity
* Decrease quantity
* Remove item
* Clear cart

Acceptance criteria:

* Cart totals are always correct
* Quantity changes update totals
* Empty cart displays correctly

---

# 19. Task 16: Address Management

Create address management.

Users should be able to:

* Add address
* Edit address
* Delete address
* Select default address

Address fields:

* Full name
* Phone
* House/building
* Street
* Area
* City
* State
* Postal code
* Address type

Address types:

* Home
* Work
* Other

Acceptance criteria:

* Address validation works
* User can select a delivery address
* Default address works correctly

---

# 20. Task 17: Checkout

Create checkout screen.

Sections:

* Delivery address
* Order items
* Price summary
* Delivery fee
* Tax
* Discount
* Final amount
* Payment method

Acceptance criteria:

* Correct order total is displayed
* User must select a valid delivery address
* User must select a payment method
* Place Order button works correctly

---

# 21. Task 18: Payment Method

Create payment method selection.

Support:

* Cash on Delivery
* Card
* UPI

Requirements:

* Payment method cards
* Selected state
* Validation

Do not implement real payment gateway integration unless explicitly required.

Acceptance criteria:

* User can select a payment method
* Selected method is shown during checkout

---

# 22. Task 19: Place Order

Implement order creation.

Order should contain:

* Order ID
* User ID
* Restaurant
* Food items
* Quantities
* Delivery address
* Payment method
* Subtotal
* Delivery fee
* Tax
* Discount
* Final total
* Order date
* Order status

Initial status:

```text
Placed
```

Acceptance criteria:

* Order is created successfully
* Cart is cleared after successful order
* User is redirected to order confirmation

---

# 23. Task 20: Order Confirmation

Create order confirmation screen.

Display:

* Success message
* Order ID
* Total amount
* Estimated delivery time
* View Order button
* Continue Shopping button

Acceptance criteria:

* Confirmation appears after successful order
* Order ID is displayed

---

# 24. Task 21: Orders Screen

Create order history screen.

Display:

* Active orders
* Previous orders
* Order ID
* Restaurant
* Date
* Total
* Status

Acceptance criteria:

* Orders are displayed correctly
* User can open order details

---

# 25. Task 22: Order Details

Create order details screen.

Display:

* Order ID
* Restaurant
* Food items
* Quantities
* Price
* Delivery address
* Payment method
* Total
* Order status

Acceptance criteria:

* Complete order information is displayed
* Order status is clear

---

# 26. Task 23: Order Tracking

Create order tracking UI.

Order stages:

```text
Order Placed
     ↓
Confirmed
     ↓
Preparing
     ↓
Out for Delivery
     ↓
Delivered
```

Display:

* Current status
* Progress indicator
* Estimated delivery time

Acceptance criteria:

* Current status is visually clear
* Previous completed stages are displayed correctly

---

# 27. Task 24: Profile

Create profile screen.

Display:

* Profile picture
* Full name
* Email
* Phone number

Actions:

* Edit profile
* Manage addresses
* Favorites
* Orders
* Settings
* Logout

Acceptance criteria:

* Profile information displays correctly
* Navigation works correctly

---

# 28. Task 25: Edit Profile

Create edit profile screen.

Allow user to change:

* Name
* Phone number
* Profile image

Requirements:

* Validation
* Save button
* Loading state
* Error handling

Acceptance criteria:

* Profile changes are saved
* Updated information appears immediately

---

# 29. Task 26: Settings

Create settings screen.

Options:

* Notifications
* Dark mode
* Language
* Privacy
* Terms and conditions
* About

Acceptance criteria:

* Settings display correctly
* Toggle options work correctly

---

# 30. Task 27: Authentication State

Implement persistent authentication state.

Requirements:

* Store authenticated user state
* Restore authentication after app restart
* Logout functionality
* Protect authenticated screens

Acceptance criteria:

* Logged-in user stays logged in after restart
* Logout clears authentication state
* Unauthenticated users cannot access protected screens

---

# 31. Task 28: API/Data Layer

Create a centralized data access layer.

Requirements:

* API service
* Repository pattern
* Models
* JSON parsing
* Request handling
* Response handling
* Error handling

Do not place API calls directly inside UI widgets.

Acceptance criteria:

* API logic is separated from UI
* Models are reusable
* Errors are handled consistently

---

# 32. Task 29: State Management

Implement centralized state management.

Manage:

* Authentication
* Restaurants
* Foods
* Favorites
* Cart
* Address
* Orders
* Profile

Avoid unnecessary global state.

Acceptance criteria:

* UI updates automatically when state changes
* Business logic remains outside widgets

---

# 33. Task 30: Loading and Error States

Add consistent states throughout the app.

Loading states:

* Skeleton/loading indicators where appropriate

Error states:

* Network error
* Server error
* Invalid data
* Authentication error

Empty states:

* Empty cart
* No favorites
* No orders
* No search results
* No restaurants

Acceptance criteria:

* No screen remains blank during loading
* Errors are understandable
* Empty states are visually clear

---

# 34. Task 31: Form Validation

Review all forms.

Validate:

* Email
* Password
* Phone
* Name
* Address
* Required fields
* Numeric values

Acceptance criteria:

* Invalid input is rejected
* Useful validation messages are displayed
* Forms cannot submit invalid data

---

# 35. Task 32: Responsive UI

Test the application on multiple mobile screen sizes.

Check:

* Small screens
* Medium screens
* Large screens
* Portrait orientation

Acceptance criteria:

* No overflow
* No clipped text
* No broken layouts
* Buttons remain accessible

---

# 36. Task 33: Code Quality

Review the entire codebase.

Check for:

* Duplicate code
* Unused imports
* Unused variables
* Poor naming
* Large widgets
* Missing error handling
* Incorrect state management
* Hardcoded values

Refactor only where necessary.

Acceptance criteria:

* Code is readable
* Code follows Flutter/Dart conventions
* No unnecessary duplication

---

# 37. Task 34: Testing

Create tests for important functionality.

Test:

* Authentication
* Form validation
* Cart calculations
* Quantity changes
* Order totals
* Favorites
* Address validation

Acceptance criteria:

* Important business logic has tests
* Tests pass successfully

---

# 38. Task 35: Flutter Analyzer

Run:

```bash
flutter analyze
```

Fix all errors.

Warnings should be reviewed and fixed where appropriate.

Acceptance criteria:

```text
flutter analyze
```

completes without errors.

---

# 39. Task 36: Build Verification

Run:

```bash
flutter pub get
flutter analyze
flutter test
flutter build apk
```

Fix any errors found during the process.

Acceptance criteria:

* Dependencies resolve successfully
* Analyzer passes
* Tests pass
* APK builds successfully

---

# 40. Task 37: Final Review

Perform a complete application review.

Check:

* Authentication
* Home
* Search
* Categories
* Restaurants
* Food details
* Favorites
* Cart
* Address
* Checkout
* Payment selection
* Orders
* Order tracking
* Profile
* Settings
* Logout

Check for:

* UI bugs
* Navigation bugs
* Data bugs
* Crashes
* Incorrect calculations
* Missing loading states
* Missing error states

---

# 41. Task 38: Final Cleanup

Remove:

* Debug prints
* Temporary files
* Unused code
* Unused dependencies
* Test data
* Development-only UI

Ensure production-ready code remains.

---

# 42. Task 39: Final Verification

Run the complete verification process:

```bash
flutter clean
flutter pub get
flutter analyze
flutter test
flutter build apk
```

Verify that the final application launches successfully.

---

# 43. Important Agent Rules

The agent MUST follow these rules:

1. Work on exactly one task per iteration.
2. Read `PRD.md` before starting work.
3. Read `progress.txt` before starting work.
4. Never modify `PRD.md`.
5. Append progress to `progress.txt`.
6. Never delete previous progress entries.
7. Do not skip unfinished tasks.
8. Do not mark a task complete unless its acceptance criteria are satisfied.
9. Run appropriate tests after implementation.
10. Fix errors before marking a task complete.
11. Do not redesign existing UI unless the task explicitly requires it.
12. Reuse existing project architecture when possible.
13. Do not introduce unnecessary dependencies.
14. Do not overwrite working functionality unnecessarily.
15. Keep changes limited to the current task.
16. Review existing code before creating new code.
17. Preserve backward compatibility where possible.
18. Do not use fake API responses when real project APIs already exist.
19. Never expose secrets, API keys, passwords, or credentials.
20. Before making destructive changes, verify the impact.

---

# 44. Definition of Done

A task is considered complete only when:

* Implementation is complete
* Acceptance criteria are satisfied
* Code compiles
* Relevant tests pass
* No new analyzer errors are introduced
* Existing functionality still works
* Progress is recorded in `progress.txt`

---

# 45. Final Project Goal

The final application should be a complete, stable, maintainable Flutter food delivery application with:

* Authentication
* Restaurant browsing
* Food browsing
* Search
* Categories
* Favorites
* Cart
* Address management
* Checkout
* Payment method selection
* Orders
* Order tracking
* Profile
* Settings
* Proper state management
* Proper error handling
* Responsive UI
* Automated testing
* Production-ready Flutter code

The agent should work incrementally and verify each task before moving to the next task.
