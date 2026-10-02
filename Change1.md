---
published: false
---

# Change 1: Update Contact Page

## Goals

- Streamline the Contact page by removing placeholder text.
- Add contact information through the approved LinkedIn link.

## Branch and scope

- Work on `update-contact-page`, created from the synced `main` branch.
- Include only `contact.md` and this planning document in the pull request.
- Keep this document unpublished so it does not become a Jekyll website page.

## Planned change

1. Remove the subtitle: “A simple place to add a preferred public contact method.”
2. Remove all existing Contact page body text, including the public-email note and the contact-method placeholder.
3. Replace that body text with a single clickable link:
   `[LinkedIn](https://www.linkedin.com/in/erin-barrett2)`.
4. Retain the Contact heading, navigation, layout, and existing page metadata other than the removed subtitle.
5. Do not add an email address or fetch information from the LinkedIn profile.

## Planned verification

- Build the Jekyll site successfully.
- Check `/contact/` in Preview.
- Confirm the removed subtitle and body text no longer appear.
- Confirm the LinkedIn link has the exact approved HTTPS destination.
- Confirm this document is not included in the generated website.
- Review the Git diff to ensure no unrelated files are included.

## Commit and pull request

- Proposed commit message: `Streamline Contact page and add LinkedIn link`
- Push `update-contact-page` to GitHub only after approval.
- Open a pull request titled `Update Contact Page` targeting `main`, only after approval.
- Do not merge the pull request without separate approval.

## Approval checkpoints

Ask for confirmation before editing the Contact page, running the build and Preview checks, committing, pushing, and opening the pull request.

## Completed edit and verification

- Removed the Contact subtitle and all previous body text.
- Replaced the body with the single approved LinkedIn link:
  `[LinkedIn](https://www.linkedin.com/in/erin-barrett2)`.
- Retained the Contact heading, navigation, layout, and remaining page metadata.
- Built the Jekyll site successfully.
- Checked `/contact/` in Replit Preview at desktop and mobile sizes.
- Confirmed the removed text no longer appears and the link has the exact approved HTTPS destination.
- Confirmed no email address was added and no information was fetched from LinkedIn.
- Confirmed this document is not included in the generated website.
- Reviewed the changes against GitHub's `main`: only `contact.md` and `Change1.md` are included.

The edit and verification are complete. Pushing the branch, opening the pull request, and merging still require separate approval.