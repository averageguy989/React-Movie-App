# 🎬 MovieApp - React Movie Search & Discovery

A modern, responsive React application that allows users to search for movies, discover trending films, and get detailed information about their favorite movies. Built with React, Vite, and integrated with TMDB API and Appwrite backend.

## 🌐 Live Demo

**🎬 [View Live Application](https://react-movie-app-lczb.vercel.app/)**

---

## ✨ Features

- **🔍 Dynamic Movie Search**: Real-time search with debouncing for optimal performance
- **📱 Responsive Design**: Mobile-first design that works on all devices
- **🎯 Trending Movies**: Display top trending movies based on search analytics
- **🔄 Search Analytics**: Track search terms and movie popularity using Appwrite
- **⚡ Fast Loading**: Optimized with Vite for quick development and fast builds
- **🎨 Modern UI**: Clean, intuitive interface with smooth animations
- **📊 Error Handling**: Graceful error handling with user-friendly messages
- **🔄 Loading States**: Smooth loading spinners and progress indicators

## 🛠️ Technologies Used

- **Frontend**: React 18, Vite
- **Styling**: Tailwind CSS
- **Backend**: Appwrite (Database & Authentication)
- **API**: TMDB (The Movie Database)
- **State Management**: React Hooks (useState, useEffect)
- **Build Tool**: Vite
- **Package Manager**: npm

## 🚀 Getting Started

### Prerequisites

- Node.js (version 16 or higher)
- npm or yarn
- Appwrite account and project
- TMDB API key

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/averageguy989/React-Movie-App.git
   cd React-Movie-App/MovieApp
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   Create a `.env` file in the root directory:
   ```env
   VITE_TMDB_API_KEY=your_tmdb_api_key_here
   VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
   VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
   VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
   ```

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to `http://localhost:5173`

## 🔧 Configuration

### Appwrite Setup

1. Create an Appwrite project
2. Set up a database with a collection for search analytics
3. Configure the following collection attributes:
   - `searchTerm` (string)
   - `count` (integer)
   - `movie_id` (string)
   - `poster_url` (string)

### TMDB API Setup

1. Visit [TMDB](https://www.themoviedb.org/settings/api)
2. Create an account and request an API key
3. Add your API key to the `.env` file

## 📱 Usage

### Search Movies
- Type in the search bar to find movies
- Results update in real-time as you type
- Search is debounced for optimal performance

### View Trending Movies
- Trending movies are displayed based on search analytics
- Movies are ranked by popularity and search frequency

### Movie Details
- Click on movie cards to view more information
- View movie posters, titles, and basic details

## 🏗️ Project Structure

```
MovieApp/
├── public/                 # Static assets
│   ├── hero-bg.png        # Hero background image
│   ├── hero.png           # Hero image
│   ├── logo.png           # App logo
│   ├── no-movie.png       # No results image
│   ├── search.svg         # Search icon
│   ├── star.svg           # Star icon
│   └── vite.svg           # Vite logo
├── src/
│   ├── components/        # React components
│   │   ├── Search.jsx     # Search functionality
│   │   └── Spinner.jsx    # Loading spinner
│   │   └── MovieCard.jsx  # Display the Movies information
│   ├── services/          # API services
│   │   └── appwrite.js    # Appwrite database operations
│   ├── App.jsx            # Main application component
│   ├── App.css            # Application styles
│   ├── index.css          # Global styles
│   └── main.jsx           # Application entry point
├── .gitignore             # Git ignore file
├── package.json           # Project dependencies
├── vite.config.js         # Vite configuration
└── README.md              # Project documentation
```

## 🔍 Key Components

### Search Component
- Handles user input with debouncing
- Integrates with TMDB API for movie search
- Updates search analytics in Appwrite

### Spinner Component
- Loading indicator with smooth animations
- Centered layout using Tailwind CSS
- Accessible with proper ARIA labels

### App Component
- Main application logic
- State management for movies and search
- Integration with external APIs

## 📊 API Integration

### TMDB API
- **Endpoint**: `https://api.themoviedb.org/3/search/movie`
- **Authentication**: API key in headers
- **Features**: Movie search, poster URLs, movie metadata

### Appwrite Backend
- **Database**: Stores search analytics and trending data
- **Collections**: Search terms, movie counts, and metadata
- **Real-time**: Updates search statistics in real-time

## 🎨 Styling

- **Framework**: Tailwind CSS
- **Design**: Modern, clean interface
- **Responsive**: Mobile-first approach
- **Animations**: Smooth transitions and loading states

## 🚀 Deployment

### Live Application
**🎬 [MovieApp Live Demo](https://react-movie-app-lczb.vercel.app/)**

### Build for Production
```bash
npm run build
```

### Deploy to Vercel/Netlify
1. Build the project
2. Upload the `dist` folder
3. Configure environment variables

**Note:** This project is currently deployed on [Vercel](https://vercel.com/) and accessible at [https://react-movie-app-lczb.vercel.app/](https://react-movie-app-lczb.vercel.app/)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [TMDB](https://www.themoviedb.org/) for providing the movie database API
- [Appwrite](https://appwrite.io/) for the backend infrastructure
- [React](https://reactjs.org/) for the amazing frontend framework
- [Vite](https://vitejs.dev/) for the fast build tool
- [Tailwind CSS](https://tailwindcss.com/) for the utility-first CSS framework

## 📞 Support

If you have any questions or need help with the project:

- Create an issue on GitHub
- Contact: [Your Contact Information]
- Project Link: [https://github.com/averageguy989/React-Movie-App](https://github.com/averageguy989/React-Movie-App)

---

**Made with ❤️ by [Chandru]**

*This project was built as part of the 100xDevs ReactJS course to learn modern web development practices.*
