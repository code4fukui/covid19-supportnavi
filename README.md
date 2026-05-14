# covid19-supportnavi

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

An open-source project that allows you to quickly create a support information navigator site, modeled after the Tokyo Metropolitan Government's "Support Information Navigator for COVID-19". This tool helps citizens and businesses find relevant administrative services through an interactive questionnaire.

## Features

-   **Interactive Questionnaire:** Guides users to the support systems that suit them through a series of questions (e.g., "Are you a business or an individual?").
-   **Thematic Browsing:** Allows users to view all available support systems grouped by theme.
-   **Data-Driven Content:** The navigator's logic and service information are loaded from two CSV files, making updates simple and code-free.
-   **Customizable Appearance:** Easily change the site's color scheme by editing CSS variables. Three themes are provided by default: Default, Light, and Dark.
-   **Accessibility Controls:** Includes built-in UI controls for changing color schemes and adjusting font size.
-   **Static Site:** Generates a full set of static HTML, CSS, and JS files that can be deployed to any static web host.

## Getting Started

### Prerequisites

-   [Node.js](https://nodejs.org/)
-   [npm](https://www.npmjs.com/)

### Installation

1.  Clone the repository to your local machine:
    ```bash
    git clone https://github.com/code4fukui/covid19-supportnavi.git
    cd covid19-supportnavi
    ```

2.  Install the required dependencies:
    ```bash
    npm install
    ```

### Running in Development Mode

To start a local development server, run:

```bash
npm start
```

This will launch a server at `http://localhost:8080`. In development mode, you can test new data by simply **dragging and dropping your updated CSV files** onto the browser window. The site will load them and update the navigator instantly.

### Building for Production

To generate the static site files for deployment, run:

```bash
npm run build
```

The complete site will be generated in the `dist/` directory. You can then upload the contents of this directory to your web host.

## Customization

The primary way to customize the navigator is by providing your own data files.

### Service Information Data

This file contains the details of each administrative service.
-   **For detailed schema and instructions, please refer to "About the administrative service information csv" in `manual.pdf`.**

### Navigation Logic Data

This file defines the questions, answers, and branching logic of the interactive navigator.
-   **For detailed schema and instructions, please refer to "About the navigation logic csv" in `manual.pdf`.**

### Color Scheme

You can modify the site's appearance by editing the CSS variable definitions in the following files:

-   `static/styles/color-def-default.css` (Standard theme)
-   `static/styles/color-def-light.css` (Light theme)
-   `static/styles/color-def-dark.css` (Dark theme)

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.