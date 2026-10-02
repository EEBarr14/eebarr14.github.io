---
published: false
---

# Change 2: Add picture of Erin to “About” page

## Goals

- Add the selected picture of Erin to the About page.
- Place the picture to the right of “Outside work.”

## Branch and scope

- Work on `add-about-page-photo`, with the public PR commit based on GitHub's synced `main`.
- Include only `about.md`, `assets/css/site.css`, `assets/images/erin-barrett-hiking.jpg`, and this planning document in the pull request.
- Keep the original upload, workspace files, and generated preview output out of the pull request.
- Keep this document unpublished so it does not become a Jekyll website page.

## Planned change

1. Add the selected photo as a browser-ready JPEG at `assets/images/erin-barrett-hiking.jpg`.
2. Preserve the full photo without cropping and remove embedded metadata from the public copy.
3. Place the image to the right of the Outside work heading and existing paragraph.
4. Add descriptive alternative text and responsive styling for desktop and mobile.
5. Retain the existing About page text, navigation, layout, and metadata.

## Planned verification

- Build the Jekyll site successfully.
- Preview `/about/` at desktop and mobile sizes.
- Confirm the selected photo appears to the right of Outside work.
- Verify that the image URL loads successfully with JPEG content.
- Confirm the existing Outside work text is unchanged.
- Confirm this document is not included in the generated website.
- Review the diff against GitHub's `main` to ensure only the four scoped files are included.

## Commit and pull request

- Proposed photo commit message: `Add picture of Erin to “About” page.`
- Push `add-about-page-photo` to GitHub only after approval.
- Open a pull request targeting `main` only after approval.
- Commit and push this planning document to the existing pull request only after separate approval.
- Do not merge the pull request without separate approval.

## Approval checkpoints

Ask for confirmation before each new step. The user's approval to prepare the preview covered the photo copy, page edit, and preview checks. Committing, pushing, opening the pull request, and merging require separate approval.

## Completed edit and verification

- Added a full-frame browser-ready JPEG of the selected photo, with embedded metadata removed.
- Placed the image to the right of the existing Outside work content.
- Added descriptive alternative text and responsive desktop/mobile styling.
- Built the Jekyll site successfully.
- Checked the About page in Replit Preview at desktop and mobile sizes.
- The user approved the preview.
- Verified that the image URL returns HTTP 200 with `image/jpeg` content and that the generated image matches the site asset.
- Confirmed the existing Outside work text is unchanged.
- Confirmed both `Change1.md` and `Change2.md` are excluded from generated website pages and the sitemap.
- Created the approved photo commit, pushed the approved branch, and opened the approved pull request.
- The pull request remains open and unmerged.

The planning-document checks are complete. Pushing this document and merging the pull request still require separate approval.