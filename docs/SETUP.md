# Setting up locally with docker(recommended)
Please note that although docker is recommended, you can also set up the project without it.
But using docker is recommended as it simplifies the setup process, and keeps the envirnment consistent without interfering with your local setup.
Kindly go through the docker installation process for your OS first.

## Prerequisites
- node.js/ nvm / volta (recommended)
- Docker
- pnpm

## Steps

1. Clone the repository.
2. Run `pnpm install` to install dependencies.
3. Run `pnpm run dev` to start the development server.

### Local Supabase Setup:
1. Run `pnpm dlx supabase init` to initialize a local Supabase project.
2. Run `pnpm dlx supabase start` to start the local Supabase server.
3. Run `pnpm dlx supabase stop` to stop the local Supabase server.

## Environment Variables

### .env.local (located in the root directory)
Contains the environment variables for the supabase setup.
- After running `pnpm dlx supabase start`, check your terminal for the Database URL and publishable Keys.
- Paste the URL into the `NEXT_PUBLIC_SUPABASE_URL`, and the publishable key into the `NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY`.

### .env (in supabase folder)
Contains the environment variables for google OAuth services.
- Setup your own OAuth credentials at [Google Cloud Console](https://console.cloud.google.com/).
- Note the secret key and client ID.
- Paste the client ID into the `SUPABASE_AUTH_GOOGLE_CLIENT_ID` and the secret key into the `SUPABASE_AUTH_GOOGLE_SECRET`.
