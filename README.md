# 🎁 Grab Bag Name Draw

A simple Secret Santa / grab bag page. Send out one link, and each friend picks their name to see who they're buying a gift for.

- Nobody draws themselves.
- Everyone is drawn by exactly one person.
- No server or database needed. It's a single `index.html` file.

## Set up your names

1. Open `index.html` (on GitHub: click the file, then the pencil icon ✏️ to edit).
2. Find the section marked `EDIT THIS PART` near the bottom.
3. Replace the sample names, and set the spending limit (or use `""` to hide it):

```js
const NAMES = [
  "Alex",
  "Bailey",
  "Casey"
];
const DRAW_CODE = "christmas-2026";
const BUDGET = "$25";
```

4. Commit the change.

To redraw everyone with new pairs, change `DRAW_CODE` to any other word. Do this **before** sending the link, because it changes everyone's match.

## Put it online with GitHub Pages

1. In your repository, go to **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Choose your branch (usually `main`) and the `/ (root)` folder, then click **Save**.
4. After a minute or two, your link appears at the top of that page, something like
   `https://your-username.github.io/your-repo-name/`

Send that link to your friends.

## Organizer view

Add `#organizer` to the end of the link to see every pair:
`https://your-username.github.io/your-repo-name/#organizer`

Keep that one to yourself.

## Good to know

- **Honor system:** someone could pick a friend's name to peek, and anyone who reads the page's code could work out the pairs.
- **Public repo = public names:** on a free GitHub account, Pages sites come from public repositories, so anyone can see your friends' names in the code. Use first names or nicknames if that matters to you.
- **Remembers on each phone:** people can come back later to check their match. A "Someone else is using this device" button lets a second person use the same phone.
