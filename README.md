# hugo-twitter-timeline

A simple Hugo shortcode for embedding a Twitter timeline, based on the Twitter
widgets code, which can be accessed via https://publish.twitter.com/ and https://platform.twitter.com/widgets.js

# Parameters

The supported parameters are
- `username`: The username of the Twitter account to embed the timeline for (required)
- `language`: The ISO 639-1 language code for the language in which to render the timeline (see [Supported languages and browsers – Twitter for Developers](https://developer.twitter.com/en/docs/twitter-for-websites/supported-languages) for more information), set automatically by Twitter if not specified
- `width`: The width of the timeline in pixels
- `height`: The height of the timeline in pixels
- `donottrack`: Whether to enable the [Do Not Track](https://developer.twitter.com/en/docs/twitter-for-websites/privacy) feature, either `true` or `false` – defaults to `true` to preserve your privacy
- `theme`: The theme to use for the timeline, either `light` or `dark` – defaults to `light`

# Usage

To use the shortcode, simply add the following to your Hugo content file(s) and/or customise as needed:

```
{{< twitter-timeline username=twitter language=en width=500 height=800 donnottrack=true theme=dark >}}
```

assuming that the shortcode is saved as `twitter-timeline.html` in your Hugo theme's `layouts/shortcodes` directory.

# License

This project is licensed under the [MIT License](LICENSE).

# Footnotes

Feel free to use it across your projects and star this repository. If you have any questions or suggestions, please feel free to open an issue or a pull request.
