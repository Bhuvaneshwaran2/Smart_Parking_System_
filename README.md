# Smart Parking System — GitHub Pages Version

This is the beginner-friendly static version of the Smart Parking Allocation and Navigation Optimization System.

## What it includes
- One-page HTML/CSS/JavaScript application
- Sample parking-space status
- Greedy-style allocation: choose the nearest available space
- Dijkstra's shortest-path algorithm on a small weighted graph
- Release an occupied parking space
- No Java backend, no MySQL, no database, no build tools

## Important storage note
All data is stored in JavaScript variables in the current browser page. Refreshing the page resets the parking status to the original sample data. This is temporary in-memory storage, not shared storage between visitors.

## Publish with GitHub Pages
1. Sign in to https://github.com/
2. Click **+** → **New repository**.
3. Name it `smart-parking-system`. Choose Public if you want to share it.
4. Create the repository.
5. Click **Add file** → **Upload files**.
6. Upload `index.html` (and this README if you want documentation).
7. Click **Commit changes**.
8. In the repository, open **Settings** → **Pages**.
9. Under **Build and deployment**, choose **Deploy from a branch**.
10. Set branch to `main` and folder to `/(root)`, then click **Save**.
11. Wait a minute or two, refresh the Pages settings, and open the published URL shown there.

For a repository named `smart-parking-system`, the URL will normally look like:
`https://YOUR-GITHUB-USERNAME.github.io/smart-parking-system/`

Replace `YOUR-GITHUB-USERNAME` with your GitHub username. The exact URL is shown in repository Settings → Pages.

## Test the site
- Click **Find and allocate nearest space**. A free space should become occupied.
- Click **Release** on an occupied space. It should become available.
- Use **Calculate shortest route** to show a route and total distance.
- Click **Reset demo data** or refresh the browser to restore the initial data.

## Limitations
- GitHub Pages only serves static files. It cannot run Java/Spring Boot.
- Each visitor has their own separate in-memory state.
- Changes disappear on refresh and are not shared between users.
- The road distances are illustrative example values for demonstrating Dijkstra's algorithm.
