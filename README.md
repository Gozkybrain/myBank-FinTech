# Fintech Bank Application

## Overview

This project is a web-based project for a fintech bank, its will include different types of account eg; `savings`, `investments`, and `loans`. The whole process involved in a bank will be carried out here including transaction of funds, investments, etc.

## Technologies Used

- **React JS**: Frontend.
- **Firebase**: Authentication and Database.
- **FontAwesome**: UI Icons.
- **Animate.Style**: Animated Concepts.
- **CSS**: Custom styling.
- **EmailJS**: Seamless Email Notification without Backend.


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

## Logic for Trade and Withdrawal
- The Trade starts by filling the form, this takes out the amount, and matches it with a corresponding plan. If the entered amount is 100 for a Basic plan with 10% profit in 24 hours, the calculation and expected profit is `(100 x 10%) x 24` then the result is added to the capital ie `240 + 100 = 340`.
- There is a credit for the profit with a pending description.
- The user role also automatically changes to investor.
- The trade option is not available for admin for security reasons, and for investor it shows that the trading is in progress.
- While the trading is in progress, it displays the pending transaction which has a date and an end date. If the end date is greater or equal to today's that then there is a claim profit button, else there is a text signifying that the trade is still in progress.
- The button to claim profit will edit the transaction and assign it to Investments from Trading, and restore the user back to their role as user.
- The Withdrawal is only available for balances based on `account: Investments`.

## Getting Started

### Prerequisites

- Node.js

- Install all dependencies `npm install`

- Start project `npm start`

### Usage of Template
- Login: Enter your email and password to log in. Only admin users have access to the full admin panel.

- Transaction: Transactions will be carried out by users.

- Logout: Click the logout button to sign out from the application.

- Add firebase information to connect to your project.
- Edit user information and transactions.


## Important

- By Default, Newly Registered users will have role as `user` and group as `cancelled`. Cancelled can not make transfer, Deactivated will make pending transfers, and Activated will be complete.

- When a User makes a withdrawal; `deactivated` means pending but group will change to `cancelled` which means do not allow. `activated` will go completed.

- During a trade; `Admins` will not be allowed to trade for security reasons, `Investor` means that a trade is currently ongoing, while `User` can carry out activities. If a user makes a  trade, onsubmit their role changes to investor signifying that their trade has not ended. When ended, the investor now clicks on the claim button which completes the transaction, sends the email, and returns the investor to user.

