# Lead Generation & Website Audit Tool

This is a Python-based tool built with [Streamlit](https://streamlit.io/) that helps users find potential clients by identifying specific technical issues on their websites.

## Features

- **Lead Discovery**: Search for businesses by Niche and Region.
- **Website Audit**: Check for:
  - Slow Page Load (> 3 seconds)
  - Missing SEO Meta Tags (Title, Description)
  - Broken Links (404s on Homepage)
- **Contact Extraction**: automatically finds email addresses on the homepage.
- **Export**: Download results as a CSV file.

## How to Run Locally

1. **Clone the repository** (if you haven't already):
   ```bash
   git clone <your-repo-url>
   cd <your-repo-folder>
   ```

2. **Install Dependencies**:
   It is recommended to use a virtual environment.
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the App**:
   ```bash
   streamlit run app.py
   ```
   The app will open in your default browser at `http://localhost:8501`.

## How to Host for Free

The easiest way to host this application for free is using **Streamlit Community Cloud**.

### Steps to Deploy on Streamlit Community Cloud:

1.  **Push your code to GitHub**:
    - Ensure your project has `app.py` and `requirements.txt` in the root directory.
    - Commit and push your changes to a public GitHub repository.

2.  **Sign up/Login to Streamlit Cloud**:
    - Go to [share.streamlit.io](https://share.streamlit.io/).
    - Sign in with your GitHub account.

3.  **Deploy the App**:
    - Click **"New app"**.
    - Select your **Repository**, **Branch** (usually `main`), and **Main file path** (e.g., `app.py`).
    - Click **"Deploy!"**.

Streamlit Cloud will install the dependencies listed in `requirements.txt` and launch your app. You will get a unique URL (e.g., `https://your-app-name.streamlit.app`) to share with others.

### Alternative Free Hosting Options:

-   **Hugging Face Spaces**: Create a new Space, select "Streamlit" as the SDK, and upload your files (or connect to GitHub).
-   **Render**: You can deploy as a Web Service (using a `startCommand` like `streamlit run app.py --server.port $PORT`), though the free tier will spin down after inactivity.
