
# Cinemate

Cinemate is a full-stack film information platform reminiscent of IMDb, developed using Nuxt.js and enriched with Tailwind CSS. Utilizing The Movie DB API, Cinemate provides users with comprehensive listings of the latest releases, popular titles, and upcoming movies, all detailed within dedicated pages. Supabase integration ensures efficient back-end management for data handling, contributing to a seamless and secure user experience.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Integration](#api-integration)
- [Supabase Setup](#supabase-setup)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Latest Releases**: Stay updated with the newest movie releases.
- **Popular Titles**: Discover the most popular movies currently trending.
- **Upcoming Movies**: Get information about movies that are soon to be released.
- **Detailed Movie Pages**: Access detailed information about each movie, including synopsis, cast, crew, and more.
- **User Authentication**: Secure user authentication and management through Supabase.
- **Responsive Design**: Enjoy a seamless experience on both desktop and mobile devices, thanks to Tailwind CSS.

## Technologies Used

- **Nuxt.js**: A powerful Vue.js framework for building server-side rendered applications.
- **Tailwind CSS**: A utility-first CSS framework for styling.
- **The Movie DB API**: Provides comprehensive movie data.
- **Supabase**: An open-source backend-as-a-service providing database and authentication.

## Installation

To get started with Cinemate, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/cinemate.git
    cd cinemate
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Set up environment variables**:
    Create a `.env` file in the root directory and add the following variables:
    ```env
    TMDB_API_KEY=your_tmdb_api_key
    SUPABASE_URL=your_supabase_url
    SUPABASE_ANON_KEY=your_supabase_anon_key
    ```

4. **Run the development server**:
    ```bash
    npm run dev
    ```

    Your application should now be running on `http://localhost:3000`.

## Usage

Once the application is up and running, you can navigate through various sections such as latest releases, popular titles, and upcoming movies. Click on any movie to view detailed information.

## API Integration

Cinemate uses The Movie DB (TMDB) API to fetch movie data. Make sure to sign up on [TMDB](https://www.themoviedb.org/) to get your API key and add it to the `.env` file.

## Supabase Setup

Cinemate leverages Supabase for backend management, including user authentication and database management. To set up Supabase:

1. Sign up on [Supabase](https://supabase.io/).
2. Create a new project.
3. Navigate to the project settings to find your API URL and anon key.
4. Add these details to your `.env` file as shown in the installation steps.

## Contributing

We welcome contributions from the community. To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature-name`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to customize this README further based on your specific project needs and preferences.
