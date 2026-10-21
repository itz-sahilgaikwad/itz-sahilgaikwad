# Install the complete GitHub profile redesign

## Files included

- `README.md` — complete profile layout, project descriptions, badges, statistics, animated headline, contribution snake, and links.
- `hero.svg` — custom header artwork (repository root).
- `about-life.svg` — about section artwork (repository root).
- `stack.svg` — custom technology panel (repository root).
- `id-dashboard.svg` — custom project showcase artwork (repository root).
- `connect.svg` — custom footer artwork (repository root).
- `.github/workflows/snake.yml` — GitHub Actions workflow that generates light and dark contribution-snake SVGs on a daily schedule.

## Install in the profile repository

Repository: `itz-sahilgaikwad/itz-sahilgaikwad`

1. Extract the ZIP.
2. In the repository's **Code** tab, use **Add file → Upload files**.
3. Upload `README.md` and the five SVG files to the repository root. To enable the contribution snake, also create `.github/workflows/snake.yml` using the included workflow file (see below).
4. Commit the changes.
5. Open **Actions** in the repository and run **Generate contribution snake** once with **Run workflow**. The workflow publishes the generated snake images to an `output` branch.
6. If GitHub Actions are disabled or restricted for the repository, enable them or remove the contribution-snake block from the README.
7. Replace `YOUR-LINKEDIN-USERNAME` and add the Snippet Manager repository URL when available.

## Important

The workflow needs permission to write to the repository's `output` branch. It only writes generated contribution SVGs to that branch; it does not change the README or application source code. GitHub statistics cards and the typing headline use external services and may occasionally be unavailable.


### Creating the workflow from GitHub's website

1. In the repository, select **Add file → Create new file**.
2. For the filename, enter `.github/workflows/snake.yml`.
3. Open `snake.yml` from the extracted `.github/workflows` folder in a text editor and copy its full contents into GitHub.
4. Commit the new file.
5. Open **Actions**, select **Generate contribution snake**, and choose **Run workflow**.
