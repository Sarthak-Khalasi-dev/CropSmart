🌾 CropSmart – AI-Powered Crop Recommendation Platform

CropSmart is a full stack web application designed to help farmers make data-driven crop selection decisions.
The platform analyzes environmental and soil conditions to recommend the most suitable crops, fertilizers, and yield predictions before sowing.

This project was built as part of a Full Stack Hackathon using modern web technologies.

📌 Problem Statement

Small and marginal farmers in India often rely on traditional knowledge, past experience, or guesswork when deciding which crops to cultivate each season. This lack of data-driven decision making frequently leads to:

Low crop yield

Poor soil health

Mismatched crops for local climate

Financial losses for farmers

Farmers rarely have access to personalized agricultural insights based on:

Soil conditions

Local climate

Rainfall patterns

Geographical location

As a result, crop choices are often inefficient and risky, especially with changing climate conditions.

💡 Proposed Solution – CropSmart

CropSmart is an AI-powered full stack platform that helps farmers choose the most suitable crop before sowing.

The system analyzes:

Soil type

Temperature

Rainfall

Location

Season

Based on these inputs, the platform provides:

🌱 Recommended crops suitable for the farmer’s land
🧪 Fertilizer suggestions for better soil productivity
📊 Yield prediction to estimate expected output
🌦 Climate-based crop compatibility

This enables farmers to make smarter and more profitable farming decisions.

⚙️ Key Features
👨‍🌾 Farmer Dashboard

A personalized dashboard where farmers can view crop recommendations and farming insights.

📍 Location-Based Analysis

Uses geographical data to analyze local climate and rainfall patterns.

🌱 Smart Crop Recommendation

Suggests the most suitable crops based on soil and environmental conditions.

📊 Yield Prediction

Provides estimated crop production for better planning.

🧪 Fertilizer Suggestions

Recommends fertilizers suitable for the selected crop and soil.

🔎 Search, Filter & Sort

Farmers can explore crop recommendations using:

Search functionality

Filtering options

Sorting options

📈 Agricultural Insights

Displays simple analytics about crop performance and farming trends.

🛠 Tech Stack
Frontend

ReactJS

Tailwind CSS

React Router

Context API / Redux

Axios

Backend

Node.js

Express.js

Database

MongoDB

MongoDB Aggregation

MongoDB Indexing

🧩 Full Stack Features Implemented
🔐 Authentication System

Signup

Login

JWT Authentication

Protected Routes

🔄 CRUD Operations

Create crop recommendations

Read crop data

Update crop data

Delete crop records

🔍 Search, Filter & Sorting

Allows users to easily find crops and insights.

📑 Pagination

Handles large datasets using:

MongoDB limit and skip

Frontend pagination UI

🌙 Theme Support

Light Mode

Dark Mode

Theme preference persistence

⚡ Debouncing

Implemented for search input to optimize API calls.

📡 REST API Integration

Frontend communicates with backend using RESTful APIs.

🧾 Form Handling & Validation

Includes:

Input validation

Error messages

Controlled components in React

📊 MongoDB Aggregation

Used for analytics such as:

Most recommended crops

Crop statistics

Farmer usage insights

🚀 MongoDB Indexing

Indexes used on:

Email (authentication)

Crop name (search)

Location fields (filtering)

🗄 Database Schema (Example)
Users
{
  name: String,
  email: String,
  password: String,
  location: String,
  role: "farmer" | "admin"
}
Crops
{
  cropName: String,
  soilType: String,
  temperatureRange: String,
  rainfallRange: String,
  fertilizer: String,
  expectedYield: Number
}
Recommendations
{
  userId: ObjectId,
  soilType: String,
  temperature: Number,
  rainfall: Number,
  recommendedCrops: [String],
  createdAt: Date
}
📁 Project Structure
CropSmart
│
├── frontend
│   ├── src
│   │   ├── components
│   │   ├── pages
│   │   ├── context
│   │   ├── hooks
│   │   └── utils
│   │
│   └── App.jsx
│
├── backend
│   ├── controllers
│   ├── models
│   ├── routes
│   ├── middleware
│   └── server.js
│
└── README.md
🚀 Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/your-username/cropsmart.git
cd cropsmart
2️⃣ Install Backend Dependencies
cd backend
npm install

Run backend server:

npm run dev
3️⃣ Install Frontend Dependencies
cd frontend
npm install

Run React app:

npm run dev
📸 Future Improvements

Real-time weather API integration

AI/ML model for crop prediction

Satellite-based soil analysis

Mobile application for farmers

Multi-language support (Gujarati / Hindi)

🌍 Impact

CropSmart can help:

Increase agricultural productivity

Reduce wrong crop selection

Improve soil management

Support sustainable farming practices

It empowers farmers with technology-driven insights to make better farming decisions.

👨‍💻 Author

Sarthak Khalasi

Aspiring Data Scientist & Full Stack Developer
Passionate about AI, agriculture, and solving real-world problems using technology.

⭐ If you like this project, consider starring the repository!
