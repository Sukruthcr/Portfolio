# Deploying this React App to Vercel

This folder contains a React app built with CRACO. It is configured for easy deployment to Vercel.

## Vercel Deployment Configuration
- The `vercel.json` file specifies:
  - Build command: `yarn build`
  - Output directory: `build` (default CRA build output)
  - Route rewrites to support client-side routing.

## Deployment Methods

### 1. Deploy Using Vercel CLI

1. Install Vercel CLI if not installed:
   ```bash
   npm install -g vercel
   ```

2. From the `app/frontend` directory, run:
   ```bash
   vercel
   ```
   This will guide you through login and project setup.

3. For subsequent deployments, run:
   ```bash
   vercel --prod
   ```

### 2. Deploy Using GitHub Integration

1. Push your project to a GitHub repository.

2. Go to https://vercel.com and sign in.

3. Import your GitHub repository into Vercel.

4. Set the project root directory to `app/frontend` in the Vercel dashboard project settings.

5. Vercel will automatically detect the `vercel.json` file and use the specified build and output.

6. Every push to the main branch will trigger an automatic deployment.

---

## Notes

- Ensure you have `yarn` or `npm` installed on your system to run the build commands.
- If you have environment variables, configure them in Vercel dashboard for production.

This completes the setup for Vercel deployment of this React app.
