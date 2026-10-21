# US Aviation Academy Student Planners

This repository publishes the US Aviation Academy student planning tools through GitHub Pages. Each planner is stored in its own folder so staff can send students a direct link to only the tool they need.

## Live student links

- [Student Training Estimator](https://studentaccounts-ar.github.io/usaa-student-tools/training-estimator/)
- [Initial Funding Planner](https://studentaccounts-ar.github.io/usaa-student-tools/initial-funding-planner/)
- [AMT Funding Planner](https://studentaccounts-ar.github.io/usaa-student-tools/AMT-Funding-Planner/)
- [AMT VA Funding Planner](https://studentaccounts-ar.github.io/usaa-student-tools/AMT-VA-Funding-Planner/)
- [AMT VA Funding Planner](https://studentaccounts-ar.github.io/usaa-student-tools/AMT-ISM-Funding-Planner/)
- [AMT VA Funding Planner](https://studentaccounts-ar.github.io/usaa-student-tools/AMT-ISM-VA-Funding-Planner/)

The two AMT folder names contain capital letters. Website paths are case-sensitive, so copy those links exactly as shown.

## Repository structure

    usaa-student-tools/
    |-- README.md
    |-- training-estimator/
    |   |-- index.html
    |-- initial-funding-planner/
    |   |-- index.html
    |-- AMT-Funding-Planner/
    |   |-- index.html
    |-- AMT-VA-Funding-Planner/
        |-- index.html

There is intentionally no root-level `index.html`. The main repository website address may therefore show a 404 page. Staff should distribute the individual planner links above.

## How GitHub Pages publishes the planners

GitHub Pages is configured to publish from the `main` branch and the repository root. This setting only needs to be configured once.

Every planner folder must contain a file named exactly `index.html`. When someone opens a folder link, GitHub automatically loads that file, so `index.html` does not appear in the student-facing web address.

The master working files may keep descriptive filenames on the US Aviation computer, such as `USAA_Student_Training_Estimator.html`. Only the published copy inside each GitHub folder must be named `index.html`.

## Before updating a planner

1. Confirm that the revised HTML file is the final approved version.
2. Open the file locally and test the calculations, buttons, printing, and mobile layout.
3. Confirm that rates, assumptions, disclosures, and resource references are current.
4. Reset or clear the form. Never upload a completed student form or saved student information.
5. Keep the descriptively named master file and a backup copy outside GitHub.
6. Identify the correct destination folder before uploading.

## Established update process

Use these steps when the revised master file still has its descriptive filename:

1. Open [the repository](https://github.com/StudentAccounts-AR/usaa-student-tools).
2. Open the folder for the planner being updated.
3. Select **Add file**, then **Upload files**.
4. Upload the revised HTML file and commit it directly to the `main` branch. Use a meaningful message, such as `Upload revised Training Estimator rates`.
5. Open the old `index.html`.
6. Use the three-dot menu or trash icon to select **Delete file**, then commit the deletion to `main`.
7. Open the newly uploaded descriptive HTML file.
8. Select the pencil icon to edit it.
9. Change the complete filename to exactly `index.html`.
10. Select **Commit changes** and commit directly to `main`.
11. Wait for the GitHub Pages deployment to finish, then test the permanent student link.

There may be a brief period between deleting the old file and renaming the new one when the planner link is unavailable. Complete the rename promptly.

## Faster replacement method

For a one-commit replacement with no intentional gap:

1. Make a copy of the approved master file on the computer.
2. Rename only the copy to `index.html`. Keep the descriptively named master file unchanged.
3. In GitHub, open the correct planner folder.
4. Select **Add file**, then **Upload files**, and upload the copied `index.html`.
5. Confirm that GitHub shows the existing file being replaced, then commit directly to `main`.
6. Delete the temporary local copy if it is no longer needed.

In Windows File Explorer, turn on **View > Show > File name extensions** before renaming. Confirm that the file is `index.html`, not `index.html.html` or simply `index`.

## After every update

1. Open the planner's permanent link.
2. Allow a few minutes for GitHub Pages to deploy.
3. If the old version appears, press **Ctrl+F5** to force a fresh browser reload.
4. Test the primary calculation workflow.
5. Test Save/Open, Print/Save PDF, and Reset/New functions when present.
6. Check the page on both a desktop-sized window and a phone-sized window.
7. Confirm that no sample student information was accidentally published.
8. Check the repository's **Actions** or **Deployments** area for a green successful deployment.

The student link does not change when `index.html` is updated.

## Troubleshooting

### The planner displays a 404 page

- Confirm that the correct folder contains a file named exactly `index.html`.
- Check spelling, capitalization, hyphens, and the `.html` extension.
- Confirm that the file is inside the intended folder rather than the repository root.
- Check **Actions** or **Deployments** and wait for publishing to complete.
- Confirm under **Settings > Pages** that the source is the `main` branch and `/(root)`.

### The old version still appears

- Wait several minutes for deployment.
- Press **Ctrl+F5**.
- Try the link in a private or InPrivate browser window.
- Confirm that the most recent commit changed the correct folder's `index.html`.

### Images, formatting, or buttons do not work

- Confirm that the published HTML file is the same approved file that worked locally.
- If the planner relies on separate images, style sheets, or scripts, upload those supporting files to the same relative locations.
- Avoid changing internal file paths during the rename.
- Review the latest commit to make sure the entire file uploaded successfully.

### The main site address shows a 404 page

This is expected while the repository has no root-level `index.html`. Use one of the direct planner links instead. A general selection page can be added at the root later without changing the individual planner links.

## Privacy and security

This repository and its GitHub Pages website are public.

- Never upload completed student forms, exported student data, passwords, access tokens, payment records, or other private information.
- Only upload blank approved planner templates and public instructions.
- Anyone can view and download the published HTML source.
- Review any planner that requests personal or payment-related information before distributing it publicly.
- Data saved by a planner in the browser may remain on that device. Staff and students should clear the planner when using a shared computer.

## Restoring an earlier version

GitHub retains the commit history. If an update introduces a problem:

1. Open the planner folder.
2. Select **History** or open the repository's commit history.
3. Locate the last known working version.
4. Retrieve that earlier `index.html`.
5. Replace the current file using the same update process.
6. Test the live link again.

Do not upload confidential information while attempting a restoration.

## Getting help from ChatGPT or Codex

Connect the GitHub account and provide this request:

> Review the README and repository structure for `StudentAccounts-AR/usaa-student-tools`, then help me update the [planner name] without changing its student link.

The assistant should inspect this README and the current repository before recommending changes.

---

Maintenance instructions last reviewed: October 9, 2026.
