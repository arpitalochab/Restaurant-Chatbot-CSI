Please take a look in the **BOT EMULATOR TEST SCREENSHOTS** folder—those images will show you exactly how the bot works in action.


# Restaurant Chatbot

A food-tech chatbot that lets users browse restaurants, make and manage reservations, place orders, track orders, and pay via Cashfree—all through the Microsoft Bot Framework Emulator.

## Tech Stack

- Node.js  
- Express  
- MongoDB (with Mongoose)  
- Microsoft Bot Framework SDK v4  
- Axios for HTTP calls  
- JSON Web Tokens (JWT) for authentication  
- Cashfree Payments Integration  

## Prerequisites

- Node.js (v16+) and npm  
- MongoDB instance (local or Atlas)  
- Bot Framework Emulator (v4+)  
- Cashfree account credentials  

## Installation

1. Clone the repo  
   ```bash
   git clone https://github.com/<your-org>/restaurant-chatbot.git
   cd restaurant-chatbot
   ```

2. Install dependencies  
   ```bash
   npm install
   ```

3. Create a `.env` file in the project root with these variables:  
   ```text
   PORT=5000
   MONGO_URI=<your_mongodb_connection_string>
   JWT_SECRET=<your_jwt_secret>
   MICROSOFT_APP_ID=<your_bot_app_id>
   MICROSOFT_APP_PASSWORD=<your_bot_app_password>
   CASHFREE_CLIENT_ID=<your_cashfree_client_id>
   CASHFREE_CLIENT_SECRET=<your_cashfree_client_secret>
   CASHFREE_BASE_URL=<your_cashfree_api_base_url>
   ```

## Running the Bot

```bash
npm run dev
```

Then open Bot Framework Emulator and connect to:  
```
http://localhost:5000/api/messages
```

## Want to See It in Action?

Check the **BOT EMULATOR TEST SCREENSHOTS** folder for real emulator screenshots demonstrating each feature.