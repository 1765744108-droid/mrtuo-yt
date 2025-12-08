<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally and deploy it online.

View your app in AI Studio: https://ai.studio/apps/drive/1q05slh6WA2cRagvmSPcw0HKeNCc8gQT4

## Run Locally

**Prerequisites:**  Node.js

1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`

## Build for Production

To create a production build of your app:

```bash
npm run build
```

This will generate a `dist` directory with optimized production files.

## Deploy Online

### Deploy to GitHub Pages

1. Make sure you have `gh-pages` installed as a dev dependency:
   ```bash
   npm install --save-dev gh-pages
   ```

2. Update the `homepage` field in `package.json` to match your GitHub repository URL:
   ```json
   "homepage": "https://<your-username>.github.io/<your-repository-name>/"
   ```

3. Run the deploy command:
   ```bash
   npm run deploy
   ```

### Deploy to Vercel

1. Sign up for a Vercel account at https://vercel.com

2. Install the Vercel CLI:
   ```bash
   npm install -g vercel
   ```

3. Run the deploy command:
   ```bash
   vercel
   ```

4. Follow the prompts to connect your repository and deploy your app.

### Deploy to Netlify

1. Sign up for a Netlify account at https://www.netlify.com

2. Install the Netlify CLI:
   ```bash
   npm install -g netlify-cli
   ```

3. Build your app:
   ```bash
   npm run build
   ```

4. Deploy to Netlify:
   ```bash
   netlify deploy
   ```

5. Follow the prompts to deploy your app.

## Project Structure

- `components/`: React components
  - `BuildingModel.tsx`: 3D model component
  - `Controls.tsx`: Control panel component
  - `Scene.tsx`: Three.js scene component
- `constants/`: Application constants
- `utils/`: Utility functions
- `types.ts`: TypeScript type definitions
- `vite.config.ts`: Vite configuration
- `package.json`: Project dependencies and scripts

## Features

- 3D model viewing and manipulation
- Drag and drop file upload for custom models
- Model rotation and translation controls
- Vertical height adjustment
- Performance monitoring

## Dependencies

- React
- Three.js
- React Three Fiber
- React Three Drei
- Use Gesture React
- Lucide React icons

## License

MIT
