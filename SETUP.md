# GitHub Profile README Setup

This package is designed for the profile repository of `Ankit522coder`.

## 1. Create the profile repository

1. Sign in to GitHub.
2. Open `https://github.com/new`.
3. Set **Owner** to `Ankit522coder` and **Repository name** to exactly `Ankit522coder`.
4. Set the repository to **Public**.
5. Select **Add a README file** and create the repository.

GitHub only displays a profile README when the repository name exactly matches the username and the repository is public.

## 2. Upload the files

Copy these files into the root of that repository:

- `README.md`
- `.github/workflows/profile-art.yml`

Commit them to the `main` branch.

## 3. Enable the workflow

1. Open the repository's **Settings** tab.
2. Open **Actions > General**.
3. Under **Workflow permissions**, choose **Read and write permissions**.
4. Save the setting.
5. Open the **Actions** tab, select **Generate profile artwork**, and click **Run workflow**.

The workflow creates two generated branches:

- `profile-3d-contrib` for the 3D contribution graph.
- `output` for the animated contribution snake.

The first run may take a minute. After it succeeds, refresh the profile README. The scheduled job updates the artwork daily.

## 4. Replace personal links

The README already uses your supplied GitHub, LinkedIn and email details. Replace any project descriptions or links with the real repository URLs when those repositories are public. The current project cards intentionally avoid inventing URLs.

The LeetCode badge from the original README was omitted because no LeetCode profile URL was provided. Add it back only after replacing it with your real profile link.

## 5. If an image does not appear

- Confirm the repository is public.
- Confirm the username is spelled `Ankit522coder` in both files.
- Confirm both workflow jobs completed successfully in **Actions**.
- Check that the `profile-3d-contrib` and `output` branches exist.
- Wait briefly for GitHub's raw image cache to refresh.

No local package installation or download is required. GitHub Actions downloads and runs the two generators automatically.
