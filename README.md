# edm.frames website + admin panel

## Files
- `index.html`: the public website
- `content.json`: ALL text, contact info and the list of frames (the admin edits this)
- `images/`: your frame photos
- `assets/`: logo files
- `admin/index.html`: your private admin panel (open `your-site-url/admin/`)

## One-time setup (about 5 minutes)
1. In your GitHub repo, upload all these files (keep the folders). Replace the old index.html.
2. Repo > Settings > Pages: Source = "Deploy from a branch", Branch = main, folder = / (root).
3. Create a token: GitHub > Settings > Developer settings > Personal access tokens > Fine-grained tokens > Generate new token.
   - Repository access: Only select repositories > choose THIS repo
   - Permissions > Repository permissions > Contents: Read and write
   - Expiration: choose 1 year. Copy the token (starts with github_pat_).
4. Open `https://YOURNAME.github.io/REPO/admin/`, paste the token, enter `YOURNAME/REPO`, branch `main`, tap Connect.

## Daily use
- Frames tab: Add new frames > pick photos > set category / caption > Publish changes.
- Reorder with the arrows, tick "Hero frame" for the big home animation, Delete to remove.
- Text & info tab: change story, about, phone, email, Facebook link etc. > Publish changes.
- The live site refreshes about 1 minute after you publish.

## Safety
- The token lives only in your browser. Anyone opening /admin/ without it sees just a login box.
- Never share the token. If lost, delete it in GitHub settings and make a new one.
