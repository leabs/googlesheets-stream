# Google Sheets Stream

This is a statically hosted JAMStack website built with Astro and deployed and updated with Vercel.

This site uses the Server Side Rendering (SSR) mode of Astro to fetch data from a Google Sheet and render it as a static site. Not only that, the site will update itself whenever a user reloads or navigates to the site and Vercel detects a change in the Google Sheet.

## Astro SSR with Vercel's Adapter

More information on Astro's SSR here: [https://docs.astro.build/en/guides/server-side-rendering/#enabling-ssr-in-your-project](https://docs.astro.build/en/guides/server-side-rendering/#enabling-ssr-in-your-project)

## OpenSheet API

[Opensheet](https://github.com/benborgers/opensheet) allows users to get Google Sheet data as JSON with no authentication required.

## Adjusting Google Sheet

Simply change the data source in `src/pages/index.astro` to your own Google Sheet. The data source is the `fetch` function in the `data` prop of the `Page` component. Copy your Google Sheet's URL and replace the URL after `https://opensheet.elk.sh/` with your own Google Sheet's URL. more information on formatting the link can be found [here](https://github.com/benborgers/opensheet#documentation)
