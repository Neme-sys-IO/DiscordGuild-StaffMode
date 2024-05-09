# Discord Staff Guild Access Snippet

## Overview

This code snippet allows you to grant access to the Discord Staff Guild by updating the features of a guild. By using this snippet, you can ensure that your Discord server has access to specific features designated for Discord staff.

## Requirements

- Access to a web browser console
- Access to the Discord web application

## Usage

1. **Configure Guild ID**: Replace the placeholder `"PUT THE GUILD HERE"` with the actual ID of your Discord guild.
   
2. **Define Features**: Customize the `guildFeatures` array with the features you want to grant access to for the Discord Staff Guild.

3. **Run the Snippet**:
   - Open your web browser.
   - Log in to the Discord web application and navigate to any server.
   - Open the developer tools by pressing `F12` or right-clicking on the page and selecting "Inspect".
   - Go to the "Console" tab.
   - Copy the code snippet and paste it into the console.
   - Press `Enter` to run the code.

## Important Note

Make sure to use this code responsibly and only grant access to the Discord Staff Guild to authorized users. Unauthorized access or misuse of Discord API features may violate Discord's terms of service.

## Code

```javascript
const GUILD_ID = "PUT THE GUILD ID HERE";

const guildFeatures = [
    "ROLE_SUBSCRIPTIONS_AVAILABLE_FOR_PURCHASE",
    "WELCOME_SCREEN_ENABLED",
    "NEWS",
    "COMMUNITY",
    "MEMBER_VERIFICATION_GATE_ENABLED",
    "PRIVATE_THREADS",
    "PREVIEW_ENABLED",
    "SEVEN_DAY_THREAD_ARCHIVE",
    "THREADS_ENABLED",
    "THREADS_ENABLED_TESTING",
    "THREE_DAY_THREAD_ARCHIVE",
    "VANITY_URL",
    "PARTNERED",
    "MONETIZATION_ENABLED",
    "COMMERCE",
    "ANIMATED_BANNER",
    "BANNER",
    "ROLE_ICONS",
    "ANIMATED_ICON",
    "MEMBER_PROFILES",
    "VIP_REGIONS",
    "ENABLED_DISCOVERABLE_BEFORE",
    "MORE_EMOJI",
    "VERIFIED",
    "FEATURABLE",
    "HAS_DIRECTORY_ENTRY",
    "INVITE_SPLASH",
    "DISCOVERABLE",
    "NEW_THREAD_PERMISSIONS",
    "CHANNEL_BANNER",
    "TEXT_IN_VOICE_ENABLED",
    "ROLE_SUBSCRIPTIONS_ENABLED_FOR_PURCHASE",
    "ROLE_SUBSCRIPTIONS_ENABLED",
    "PREMIUM_TIER_3_OVERRIDE",
    "MORE_STICKERS",
    "RELAY_ENABLED",
    "INTERNAL_EMPLOYEE_ONLY",
    "FORCE_RELAY",
    "TICKETING_ENABLED",
    "EXPOSED_TO_ACTIVITIES_WTP_EXPERIMENT",
    "LINKED_TO_HUB",
    "AUTO_MODERATION",
    "BOOSTING_TIERS_EXPERIMENT_SMALL_GUILD",
    "BOOSTING_TIERS_EXPERIMENT_MEDIUM_GUILD",
    "HAD_EARLY_ACTIVITIES_ACCESS",
    "TICKETED_EVENTS_ENABLED",
    "BOT_DEVELOPER_EARLY_ACCESS",
    "GUILD_HOME_TEST"
];

// Find and update guild features
(webpackChunkdiscord_app.push([[''],{},e => {
    m = [];
    for (let c in e.c) m.push(e.c[c]);
}]), m)
    .find(m => m?.exports?.default?.getGuildCount)
    .exports.default
    .getGuild(GUILD_ID)
    .features = new Set(guildFeatures);
```

## License

This code is provided under the [MIT License](https://opensource.org/licenses/MIT).
