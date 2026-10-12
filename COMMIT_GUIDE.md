# Applying the changes and creating incremental commits

These updated files are a replacement for the corresponding files in your existing `Shaniel-MPOFU` repository. Keep `PROMPT_LOG.md` and any other existing files.

## 1. Back up and copy the files

1. Download and extract this package.
2. Open your existing local `Shaniel-MPOFU` repository in VS Code.
3. Copy `index.html`, `style.css`, and `README.md` from this package into the repository, replacing those three files.
4. Review the changes in Source Control before committing.

## 2. Create honest, incremental commits

The final versions in this package contain all the styling changes. To make a genuine incremental commit history, stage and commit related hunks in Git rather than making several commits of the same complete snapshot.

In VS Code:
1. Open **Source Control**.
2. Select `style.css` and use the inline diff to stage the box-model and typography changes first. Commit with `Refine CSS box model and typography`.
3. Stage the navigation-related changes next and commit with `Add responsive Flexbox navigation`.
4. Stage the skills-grid changes and commit with `Implement responsive CSS Grid for skills`.
5. Stage the media-query changes and commit with `Add mobile-first media queries`.
6. Stage the Tailwind markup changes in `index.html` and commit with `Apply Tailwind utilities to header and contact form`.
7. Stage the README changes and commit with `Document responsive design and testing`.

If the files are already fully changed in your working tree, use the **Stage Selected Ranges** option in the diff where available. Do not create commits that do not contain the changes described by their messages.

## 3. Test before pushing

Run the page with VS Code Live Server or another local server. Use browser Developer Tools to test widths of 375px, 768px, and 1280px. Check for horizontal scrolling, broken navigation, text overflow, form overflow, and browser-console errors. Update the README with the actual test results.

## 4. Push to GitHub

Once the commits are complete, use VS Code's **Sync Changes** or **Push** command, or run:

```bash
git push origin main
```

If your default branch is not `main`, use the branch name shown by `git branch --show-current`.
