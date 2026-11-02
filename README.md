# Naeem

Portfolio site for Naeem Ashraf, Social Media Manager.

Live site: https://naeemdev8-dev.github.io/Naeem/

## Content rules

These apply to every update.

- **Brand:** Daiichi Technologies is the only brand shown.
- **Client names:** no client names anywhere, except the one testimonial below.
- **Testimonials:** the only one allowed is Muhammad Nadeem (spelled N-a-d-e-e-m), Daiichi Technologies.
- **No made-up proof:** never add reviews, ratings, results or client names that aren't real and approved by the site owner.

## Add or change samples

Click **+ Add video or image** above the samples on the site. It only shows in a browser where you've connected your token. On a new device, click **Manage samples** at the bottom of the site, or go to https://naeemdev8-dev.github.io/Naeem/admin.html. Then paste your GitHub access token if asked, and add, edit, reorder or remove samples. Changes appear on the site within a few minutes.

- Videos: MP4 or WebM, up to 50 MB each. Vertical (9:16) fits best.
- Images: JPG, PNG or WebP, up to 10 MB each.

To create the token, go to https://github.com/settings/personal-access-tokens/new, select only the `Naeem` repository, and give it **Contents: Read and write**. Keep it private, like a password.

Uploads are stored in `samples/` and listed in `videos.json`.

## Change the page itself

1. Run `git pull` first, because uploads from the samples page change the repo.
2. Edit `index.html`.
3. Check the page against the content rules above, and open it in a browser.
4. Publish:

   ```powershell
   git add .
   git commit -m "describe the change"
   git push
   ```

5. Open the live site after a few minutes and confirm the change is there.

`.gitignore` only lets `videos/daiichi-technologies.*` be uploaded from `videos/`. Other files in that folder stay on your computer.

Full checklist: [CLAUDE.md](CLAUDE.md)
