# Chess.com Profile Plugin for Micro.blog

A simple Micro.blog plugin that displays your Chess.com profile with ratings and a challenge button using the Chess.com public API.

## Features

- Display Chess.com avatar, username, and title
- Show current ratings for Rapid, Blitz, Bullet, and Daily games  
- Customizable challenge button
- Clean black and white design
- Responsive layout
- No API key required

## Installation

1. Download or clone this plugin to your Micro.blog plugins directory
2. In your Micro.blog settings, navigate to the plugin configuration
3. Enter your Chess.com username
4. Optionally customize the challenge button text

## Configuration

The plugin requires two settings:

- **Chess.com Username**: Your Chess.com username (required)
- **Challenge Button Text**: Custom text for the challenge button (optional, defaults to "Challenge me on Chess.com")

## Usage

Add the shortcode anywhere in your blog posts or pages:

```
{{< chessprofile >}}
```

You can also override the username for a specific instance:

```
{{< chessprofile username="hikaru" >}}
```

## Example Output

The plugin displays:
- Profile picture and name
- Chess title (GM, IM, etc.) if applicable  
- Location
- Current ratings in a grid format
- Challenge button linking directly to Chess.com

## Files

- `plugin.json` - Plugin configuration and settings
- `layouts/shortcodes/chessprofile.html` - Hugo shortcode template
- `chess-profile.css` - Styling for the profile widget
- `README.md` - This documentation

## Requirements

- Micro.blog hosting
- Valid Chess.com username
- Internet connection for API calls

## API Usage

This plugin uses the Chess.com Published Data API which is free and requires no authentication. API calls are made at build time, so there's no impact on page load speed.

## Troubleshooting

If the profile doesn't display:
1. Check that the Chess.com username is spelled correctly
2. Ensure the username exists on Chess.com
3. Verify the user's profile is public

## Version

1.0 - Initial release