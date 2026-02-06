# Deployment Guide

Since this is a static website (HTML/CSS/JS), it is very easy to deploy for free. Here are the two best options:

## Option 1: Netlify Drop (Easiest & Fastest)
*No command line required.*

1.  Go to [app.netlify.com/drop](https://app.netlify.com/drop).
2.  Drag and drop the folder `will-you-be-my-valentine-main` onto the box on the webpage.
3.  Netlify will instantly upload and deploy it.
4.  You will get a generated URL (like `peaceful-galaxy-123.netlify.app`).
5.  (Optional) click "Site settings" to change the site name to something more personal.

## Option 2: GitHub Pages (Best for long term)
*Requires a GitHub account.*

1.  **Initialize Git**:
    Open your terminal in the project folder and run:
    ```bash
    git init
    git add .
    git commit -m "Initial commit"
    ```

2.  **Create a Repository on GitHub**:
    - Go to GitHub.com and create a new public repository (e.g., `my-valentine`).
    - *Do not* initialize it with README/gitignore (you already have them).

3.  **Push Code**:
    Follow the instructions GitHub gives you to "push an existing repository...":
    ```bash
    git remote add origin https://github.com/YOUR_USERNAME/my-valentine.git
    git branch -M main
    git push -u origin main
    ```

4.  **Enable Pages**:
    - Go to the repository **Settings** > **Pages**.
    - Under "Build and deployment" > "Source", select **Deploy from a branch**.
    - Select **main** branch and save.
    - Your site will be live at `https://YOUR_USERNAME.github.io/my-valentine/`.
