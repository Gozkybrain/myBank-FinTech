# Fintech Bank Application

## Overview

This project is a web-based project for a fintech bank, its will include different types of account eg; `savings`, `investments`, and `loans`. The whole process involved in a bank will be carried out here including transaction of funds, etc.

## Technologies Used

- **React JS**: Frontend.
- **Firebase**: Authentication and Database.
- **FontAwesome**: UI Icons.
- **Bootstrap**: Responsive Layouts.
- **CSS**: Custom styling.


## Completed components

- GetUser: to display authenticated user on default route
- SideBar: to display the menu item eg. balance for pc view
- GetAuth: to handle authentication ie login and registration
- Loader: to create a loading animation for aesthetics
- MobileNav: to display quick navigation for mobile
- user/Deposit: to handle deposit with account number
- user/Investment: to display investment plans and deposit with crypto
- user/MyCard: handles application of card and provides application number
- user/Loans: displays loan requirements
- user/Transaction: displays the transaction history
- user/Transfer: handles the transfer form
- user/UserInfo: serves as the user profile

## Features

1. **User Authentication**:
   - Login functionality using Firebase Authentication.

2. **Responsive Design**:
   - Sidebar navigation for desktop screens.
   - Hamburger menu for mobile screens.
   - Mobile navigation that slides in from the right.

3. **User Management**:
   - Transfer of Funds.
   - Application for Cards.
   - Investment Offer.
   - Loan Offers.

## Getting Started

### Prerequisites

- Node.js

- Install all dependencies `npm install`

- Start project `npm start`

### Usage
- Login: Enter your email and password to log in. Only admin users have access to the full admin panel.

- Transaction: Transactions will be carried out by users.

- Logout: Click the logout button to sign out from the application.

- Add firebase information to connect to your project.
- Edit user information and transactions.

## Future Upgrades
- Different Currencies.
- User Investment Plan System
- Upgrading to Blaze Plan to deploy functions for proper admin usage.
