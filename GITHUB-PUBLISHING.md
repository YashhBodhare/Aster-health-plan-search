# Publish this project on GitHub

The workspace folder is initialized as a local Git repository on the `main` branch. The downloadable ZIP excludes Git metadata; if you use the ZIP, initialize Git after extracting it. No GitHub remote is configured in this session.

## Create the repository

1. Create a new empty repository named `Aster-Health-Plan-Search` in your GitHub account. Start it as **private**. Do not add a second README, license, or `.gitignore`; the project folder already contains these files.
2. If you use the workspace folder, open a terminal there. If you extracted the ZIP, initialize Git first:

   ```bash
   git init -b main
   ```

3. Add the GitHub remote, stage the files, commit, and push:

   ```bash
   git remote add origin https://github.com/YOUR-USERNAME/Aster-Health-Plan-Search.git
   git add .
   git commit -m "Add Aster Health BA case study"
   git push -u origin main
   ```

4. Copy the remaining deliverables listed in `DELIVERABLES.md` into the suggested folders, then update that inventory with relative links. Commit the additions.
5. Review survey labels, privacy, brand/asset permissions, and open decisions before changing repository visibility.

GitHub is useful for the polished portfolio, change history, and reviewable documentation. Keep editable working drafts and original large files in Google Drive if that is where you collaborate; copy reviewed, sanitized versions into GitHub. Avoid maintaining competing edits in both places.
