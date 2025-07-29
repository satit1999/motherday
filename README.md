# Satit Udomseuksa School - Mother's Day Event Confirmation

This web application provides a form for parents to confirm their attendance for the Mother's Day 2025 event at Satit Udomseuksa School.

## Technology Stack

- **Framework:** React
- **Language:** TypeScript
- **Build Tool:** Vite
- **Styling:** Tailwind CSS (via CDN)
- **Backend:** Google Apps Script (connected to Google Sheets)

## Setup and Local Development

To run this project on your local machine, you need to have [Node.js](https://nodejs.org/) and npm installed.

1.  **Clone the repository:**
    Get the code from your GitHub repository onto your computer.

2.  **Install dependencies:**
    This command will download all the necessary packages like React and Vite. Open a terminal in the project folder and run:
    ```bash
    npm install
    ```

3.  **Run the development server:**
    This will start a local server, usually at `http://localhost:5173`. The website will automatically reload when you make changes to the code.
    ```bash
    npm run dev
    ```

## Deployment

This project is configured for easy deployment on modern hosting platforms like **Vercel** or **Netlify**.

1.  **Push your code to a GitHub repository.**

2.  **Connect your GitHub repository to Vercel:**
    - Sign up for a free account at [vercel.com](https://vercel.com) using your GitHub account.
    - Click "Add New..." -> "Project".
    - Import the repository from GitHub.
    - Vercel will automatically detect that this is a Vite project. It will use the `npm run build` command to prepare the files for production.
    - Click **"Deploy"**.

3.  **That's it!** Vercel will build and deploy your site, providing you with a live URL (e.g., `your-project.vercel.app`).

### Backend Configuration

The form submissions are handled by a **Google Apps Script** linked to a Google Sheet.

- The URL for this script is stored in the `constants.ts` file.
- **IMPORTANT:** Ensure the `SCRIPT_URL` in `constants.ts` is the correct "Web app" URL you received after deploying your Google Apps Script. If this URL is incorrect or a placeholder, the form will not work.
