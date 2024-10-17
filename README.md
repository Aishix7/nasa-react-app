# nasa-react-app
 Build a React.JS app with the Nasa API
Here’s a README for your APOD (Astronomy Picture of the Day) React project:

---

# APOD React Project

This project is a React application that fetches and displays NASA's Astronomy Picture of the Day (APOD) using NASA's public API. It also provides a description and additional information about the APOD, and allows users to view the image in full screen with further details in a sidebar.

**Live Demo:** [APOD React Project](https://apod-react-project28.netlify.app/)

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [File Structure](#file-structure)
- [API Reference](#api-reference)
- [Future Enhancements](#future-enhancements)

## Features

- **Display APOD**: Fetches and displays the Astronomy Picture of the Day from NASA's API.
- **Local Cache**: Uses `localStorage` to cache the APOD data to avoid multiple API calls on the same day.
- **Modal View**: Displays detailed information about the image in a sidebar modal, which users can toggle on and off.
- **Responsive Design**: Works across multiple devices and screen sizes.

## Technologies Used

- **React**: A JavaScript library for building user interfaces.
- **CSS**: Used for styling components.
- **NASA APOD API**: For fetching Astronomy Picture of the Day data.
- **Font Awesome**: For icons.
- **Netlify**: For project deployment.

## Setup Instructions

### Prerequisites
Before you begin, ensure you have the following tools installed on your machine:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/apod-react-project.git
   ```

2. Navigate to the project directory:
   ```bash
   cd apod-react-project
   ```

3. Install the project dependencies:
   ```bash
   npm install
   ```

4. Create a `.env` file in the root directory to store your NASA API key:
   ```bash
   VITE_NASA_API_KEY=your_nasa_api_key
   ```
   You can get an API key by registering on NASA's [API website](https://api.nasa.gov/).

5. Start the development server:
   ```bash
   npm run dev
   ```

6. Open your browser and go to:
   ```
   http://localhost:5173/
   ```

### Build for Production

To create a production build, run:

```bash
npm run build
```

This will create a `dist` folder with the optimized app ready for deployment.

## File Structure

The project directory structure looks like this:

```bash
src
├── components
│   ├── Footer.jsx        # Footer component displaying title and info button
│   ├── Main.jsx          # Main component showing APOD image
│   ├── SideBar.jsx       # Sidebar component displaying detailed info about APOD
├── App.jsx               # Main app logic and component rendering
├── main.jsx              # Entry point that renders App component
├── index.css             # Global styles for the project
.eslint.config.js         # ESLint configuration for the project
index.html                # HTML template file
vite.config.js            # Vite configuration for the project
```

## API Reference

This project uses the [NASA APOD API](https://api.nasa.gov/). 

**Endpoint**: `https://api.nasa.gov/planetary/apod?api_key=YOUR_API_KEY`

### Example API Response
```json
{
  "date": "2022-10-05",
  "explanation": "Explanation about the image...",
  "hdurl": "https://apod.nasa.gov/apod/image/2210/Image.jpg",
  "title": "Astronomy Picture Title"
}
```

## Future Enhancements

- **Loading States**: Improve the loading experience with more detailed loading animations.
- **Error Handling**: Add more comprehensive error messages when the API request fails.
- **Search Feature**: Allow users to search for previous APODs by date.

---

Feel free to customize and expand the README based on your project's needs! Let me know if you'd like to add more sections.
