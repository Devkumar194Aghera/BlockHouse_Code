# Interactive Analytics Dashboard

This project is an **Interactive Analytics Dashboard** built using **React**, **Chart.js**, **Axios**, and **Tailwind CSS**. It displays various types of charts (Line, Bar, Pie, and Candlestick) by fetching dynamic data from a backend API.

## Table of Contents

- [Getting Started](#getting-started)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [Approach and Thought Process](#approach-and-thought-process)

## Getting Started

To get a local copy up and running, follow these steps.

### Prerequisites

- **Node.js** installed on your machine
- **npm** or **yarn** package manager
- A running backend server providing API endpoints for the chart data

### Installing Dependencies

Navigate to the project directory and install the required dependencies:

```bash
npm install
# or
yarn install
```

## Running the Application

To run the application locally, use:

```
npm run dev
# or
yarn dev
```

The application will be available at http://localhost:3000.

## Backend API

Ensure that your backend server is running and provides the following endpoints:

- **/api/line-chart-data/**
- **/api/bar-chart-data/**
- **/api/pie-chart-data/**
- **/api/candlestick-data/**

Each endpoint should return data in JSON format for the respective charts.

## Features

- Responsive Layout: The dashboard adapts to different screen sizes.
- Real-time Data Fetching: Uses Axios to fetch data dynamically from the backend.
- Interactive Charts: Displays Line, Bar, Pie, and Candlestick charts using Chart.js and React-ApexCharts.
- Elegant UI: Styled using Tailwind CSS for a clean and modern look.
- Error Handling: Displays a user-friendly message if the backend fails to provide data.

## Technologies Used

- **React**: JavaScript library for building user interfaces.
- **Next.js**: Framework for server-side rendering.
- **Chart.js**: JavaScript library for creating charts.
- **React-ApexCharts**: React wrapper for ApexCharts, used for Candlestick chart.
- **Tailwind CSS**: Utility-first CSS framework for styling.
- **Framer Motion**: Used for smooth animations.
- **Axios**: Promise-based HTTP client for fetching data from the
  backend
- **ApexCharts**: For rendering Candlestick charts.

## Setup Instructions

1. Go Inside the Frontend Folder:

```
cd frontend
```

2. Install dependencies:

```
npm install
# or
yarn install
```

3. Run the frontend application:

```
npm run dev
# or
yarn dev
```

4. **Configure Backend and Run**: Ensure your backend server is up and running with the necessary API routes as described above by writing below code inside terminal inside the backend folder

```
python manage.py runserver
```

5. Open the browser: Navigate to http://localhost:3000 to view the application.

## Approach and Thought Process

- **Modular Components**: Each chart (Line, Bar, Pie, Candlestick) is built as a separate React component to maintain modularity and reusability.

- **Dynamic Data Fetching**: Axios is used to asynchronously fetch chart data from the backend, ensuring that the UI remains responsive even when loading large datasets.

- **Responsive Design**: Tailwind CSS is used to create a fully responsive layout, ensuring a smooth experience on both desktop and mobile devices.

- **Error Handling**: The application handles scenarios where the API fails to return data by displaying an error message instead of crashing.

- **Animation**: Framer Motion is used to add subtle animations to the loading state and charts, enhancing user experience.
