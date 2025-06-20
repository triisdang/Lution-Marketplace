

<p align="center">
  <img src="https://raw.githubusercontent.com/triisdang/Lution-Mods/refs/heads/main/Assets/thumbnails/LT_MARKETPLACE2.svg" width="420">
</p>
<sub>pls give the Lution repo a star i'm broke lol</sub>

<div align="center">

[![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/BXT7FYjTBa)

</div>

<img src="https://raw.githubusercontent.com/Lutionhq/Lution/refs/heads/latest/md/bar.png" style="width: 100%;">

# How to Create Your Own Provider

### 1. Fork this repo

Click the **Fork** button at the top of the page to get started.

### 2. Add your mod or theme

* Drop your **mod** files into: `Assets/Mods/Content/`
* Drop your **theme** files into: `Assets/Themes/Content/`
* Make sure to include a thumbnail image too!

<img src="https://raw.githubusercontent.com/Lutionhq/Lution/refs/heads/latest/md/bar.png" style="width: 100%;">

### 3. Update the config so Lution knows what to load

#### Step 1: `content.json`

You need to tell Lution what each mod or theme is.

**For mods:**
Edit `Assets/Mods/content.json`

**For themes:**
Edit `Assets/Themes/content.json`

Example format:

```json
[
  {
    "title": "My Mod",
    "body": "My first ever mod",
    "image": "https://yourimage.com/image.png",
    "button": "Download",
    "creator": "you",
    "version" : "version-xxxxxxxxxxxxxxxx",
    "sb": "unknown"
  }
]
```

**What each field means:**

* `title`: Name of the mod/theme
* `body`: Short description
* `image`: Thumbnail image URL (GitHub, Catbox, etc.)
* `button`: Just leave as "Download"
* `creator`: The creator of the mod/theme
* `version` : The version that compatible with the mod/theme
* `sb`: Stability status (`stable`, `unstable`, or `unknown`)

Same structure applies for themes.

<img src="https://raw.githubusercontent.com/Lutionhq/Lution/refs/heads/latest/md/bar.png" style="width: 100%;">

#### Step 2: `info.json`

This tells Lution the actual file paths for your mods/themes.
**Example for mods (`Assets/Themes/info.json`):**

```json
[
  { "name": "My Mod", "path": "Assets/Mods/Content/mymods.zip" }
]
```

**Important:**

* The `"name"` must match exactly with the `"title"` in `content.json`
* The `"path"` is the full path to your `.zip` file in the repo

<img src="https://raw.githubusercontent.com/Lutionhq/Lution/refs/heads/latest/md/bar.png" style="width: 100%;">

### 4. Config the Marketplace setting

When you're done, go to **Marketplace Settings** and set your marketplace provider name to your repo. (e.g. `YourUser/Lution-Marketplace`)

<img src="https://raw.githubusercontent.com/Lutionhq/Lution/refs/heads/latest/md/bar.png" style="width: 100%;">

