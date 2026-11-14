# Deploying the Undula application

Undula is a static HTML/CSS/JavaScript application. Its data and artwork are bundled in the repository; live catalogue queries run in the browser. No application server or database is required.

## Import on Vercel

1. Create a Vercel project by importing `MohamedO6/Undula` from GitHub.
2. Use branch `main` and repository root `.`.
3. Select framework **Other**. `vercel.json` already sets `framework` to `null`, `outputDirectory` to `.`, and empty installation/build commands.
4. Deploy the application. No frontend environment variables are required for the bundled app or public NASA preview lookup.

These settings follow Vercel's [static-project build configuration](https://vercel.com/docs/builds/configure-a-build) and [vercel.json reference](https://vercel.com/docs/project-configuration/vercel-json).

The repository does not include a presentation, pitch video or film kit. `.vercelignore` also excludes scientific authoring scripts and documentation from CLI uploads; they remain available in GitHub for inspection and reproduction.

## Check the deployed result

- Open the root page and enter the explorer.
- Open a location, switch between model and radar views, and inspect the source links.
- Enable sound through a click or tap, then play the model timeline.
- Open the Nile Delta seasonal chart and its downloadable paired values.
- Try Astrounit's “Find radar here” action over land. Results depend on current catalogue coverage.
- Check Then & Now, Sea 2100 and the Interference Lab.

The application uses public external services for maps, catalogue discovery and evidence-chain inspection. Their availability is separate from the static deployment. Rendering depends on browser support for WebGL, Canvas, ES modules and the optional Web Audio/Web Speech APIs.

## Local preview

```sh
python -m http.server 5173 --bind 127.0.0.1
```

Open `http://127.0.0.1:5173/`. Do not use a `file://` URL for the application, because module imports and fetched JSON require HTTP serving.
