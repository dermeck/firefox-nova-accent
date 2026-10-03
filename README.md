# Firefox Accent Color
Recolors Firefox Nova's violet accent to any color you choose, using one editable base color (defaults to OS accent color).

1. **Enable custom stylesheets:** open `about:config` and set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`.
2. **Find your profile folder:** open `about:profiles` and click "Open Folder" next to the Root Directory of the profile marked "in use". Typical locations:
  - Windows: `%APPDATA%\Mozilla\Firefox\Profiles\<profile>`
  - macOS: `~/Library/Application Support/Firefox/Profiles/<profile>`
  - Linux: `~/.mozilla/firefox/<profile>`
  - Flatpak: `~/.var/app/org.mozilla.firefox/.mozilla/firefox/<profile>`
  - Snap: `~/snap/firefox/common/.mozilla/firefox/<profile>`
3. **Copy the files:** create a `chrome` folder inside the profile folder if it doesn't exist, and put `color.css`, `userChrome.css` (if needed) and `userContent.css` in it.
4. **Pick your color:** edit `--color` at the top of `color.css`.
5. **Restart Firefox**

`userChrome.css` styles the browser UI (toolbar, tabs). `userContent.css` styles built-in pages like `about:support` and `about:preferences`.

Tested on Firefox version 127 (Nova enabled).