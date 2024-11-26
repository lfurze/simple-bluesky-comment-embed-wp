
# Bluesky Comments Embed

This project provides an easy way to embed Bluesky comments for any specific post directly into your website or application. Simply supply the URL of the Bluesky post, and the embed will automatically resolve the necessary information to display the comments.

## How It Works

- Input a **Bluesky post URL** (e.g., `https://bsky.app/profile/leonfurze.com/post/3laviqinqh22x`).
- The script fetches the DID and constructs the required URI automatically.
- Comments are fetched using the Bluesky public API and displayed in a styled, nested format.

## Getting Started on WordPress

1. Open the page or post editor in WordPress.
2. Add a **Custom HTML Block** to the desired location on the page.
3. Copy the full HTML code from the `index.html` file and paste it into the HTML block.
4. Replace the `postUrl` variable in the `<script>` section with your desired Bluesky post URL:

   ```javascript
   const postUrl = "https://bsky.app/profile/leonfurze.com/post/3laviqinqh22x";
   ```

5. Save or publish your post/page. The comments will dynamically appear when the page is loaded.

## For Local Testing

1. Clone or download this repository.

   ```bash
   git clone https://github.com/your-username/bluesky-comments-embed.git
   cd bluesky-comments-embed
   ```

2. Open the `index.html` file in any modern web browser to test it.

## Customization

You can adjust the following:
- **Styling:** Modify the CSS in the `<style>` section of `index.html` to fit your design.
- **Comments Section:** Add additional features like custom sorting or loading spinners.

## Example Post

For testing, you can use this placeholder Bluesky post URL:

```
https://bsky.app/profile/placeholder.did/post/placeholder-key
```

Replace this in the `postUrl` variable in the `<script>` section.

## Features

- Fetches comments dynamically using the Bluesky public API.
- Supports nested replies and displays author details (including profile pictures).
- Simple to configure—only a Bluesky post URL is required.

## Dependencies

None—this embed is self-contained and only uses modern JavaScript.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more information.

---

### Author
Created by [Your Name]. For questions or contributions, feel free to submit an issue or pull request.
