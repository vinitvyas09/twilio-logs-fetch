# Twilio Logs Fetch

A modern Next.js application for fetching, viewing, and downloading Twilio call and message logs with a sleek, dark-themed interface.

## 🚀 Features

- **📊 Fetch Logs**: Retrieve call and message logs from your Twilio account
- **🔍 Filter Logs**: Select log type (messages, calls, or both) and set the number of logs to display
- **💾 Download Logs**: Save logs locally in JSON format
- **🎨 User-Friendly UI**: Responsive design with smooth animations and dropdown menus

## 🛠️ Getting Started

### Prerequisites

- Node.js (v14 or later)
- Twilio Account (Account SID and Auth Token)

### Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/twilio-logs-download.git
   cd twilio-logs-download
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

3. **Configure Environment Variables:**
   Create a `.env.local` file in the root directory:
   ```
   TWILIO_ACCOUNT_SID=your_account_sid
   TWILIO_AUTH_TOKEN=your_auth_token
   ```

### Running the Application

1. Start the development server:
   ```bash
   npm run dev
   ```
2. Access the app at `http://localhost:3000`

## 🏗️ Architecture Overview

### Backend (`app/api/twilio/route.ts`)

- **API Endpoint:** `/api/twilio`
- **Functionality:**
  - Fetches messages and calls from Twilio based on `limit` and `type` query parameters
  - Utilizes Twilio's Node.js SDK for API interactions
  - Handles errors and missing credentials gracefully

### Frontend (`app/page.tsx`)

- **Components:**
  - Input fields for setting the number of logs to fetch
  - Dropdown menus for selecting log type and save options
- **Features:**
  - Responsive grid layout for log display
  - Loading spinner for data fetching indication
  - Smooth animations powered by framer-motion

## 🛠️ Technologies Used

- **Next.js & TypeScript**: For robust full-stack development
- **Tailwind CSS**: For rapid and consistent styling
- **Twilio SDK**: For seamless integration with Twilio services

## 📚 Documentation

For more details on Twilio's data export capabilities, visit the [Twilio Bulk Export Documentation](https://www.twilio.com/docs/usage/bulkexport).

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
