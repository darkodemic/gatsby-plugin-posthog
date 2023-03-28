# gatsby-plugin-posthog

![npm](https://img.shields.io/npm/v/gatsby-plugin-posthog?style=plastic)

A simple gatsby plugin to add [posthog](https://posthog.com/) analytics to your site. Automatically tracks all the pageviews and clicks.

This is a fork of an official fork, that includes updates to `package.json` to make it compatible with Gatsby 4.

I have not tested it with Gatsby version 5, so I am not going to bump the version number for it.

## Install

`yarn add gatsby-plugin-posthog`

or

`npm install --save gatsby-plugin-posthog`

## How to use

```javascript
// In your gatsby-config.js
module.exports = {
  plugins: [
    {
      resolve: `gatsby-plugin-posthog`,
      options: {
        // Specify the API key for your Posthog Project (required)
        apiKey: "YOUR_POSTHOG_ANALYTICS_API_KEY",
        // Specify the app host if self-hosting (optional, default: https://app.posthog.com)
        apiHost: "YOUR_POSTHOG_APP_HOST_URL",
        // Puts tracking script in the head instead of the body (optional, default: true)
        head: true,
        // Enable posthog analytics tracking during development (optional, default: false)
        isEnabledDevMode: true,
        // Pass custom variables to posthog.init() (optional)
        initOptions: {
          // ...
        }
      },
    },
  ],
}
```

## Questions?

### [Join our Slack community.](https://join.slack.com/t/posthogusers/shared_invite/enQtOTY0MzU5NjAwMDY3LTc2MWQ0OTZlNjhkODk3ZDI3NDVjMDE1YjgxY2I4ZjI4MzJhZmVmNjJkN2NmMGJmMzc2N2U3Yjc3ZjI5NGFlZDQ)
