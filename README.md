<p align="center">
  <h1 align="center">Live Streaming(Twitch Clone)</h1>
 </p>

### Fullstack Twitch Clone: Next.js 14, Live streaming, React, Prisma, Tailwind, MongoDB

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [Key Features](#key-features)
- [Prerequisites](#prerequisites)
- [Start the app](#start-the-app)
- [How to setup the initial project](#how-to-setup-the-initial-project)
- [Contact](#contact)

This is a repository for Fullstack Twitch Clone: Next.js 14, Livestreaming, React, Prisma, Tailwind, MongoDB.

### Features:

- 📡 Streaming using RTMP / WHIP protocols
- 🌐 Generating ingress
- 🔗 Connecting Next.js app to OBS / Your favorite streaming software
- 🔐 Authentication
- 📸 Thumbnail upload
- 👀 Live viewer count
- 🚦 Live statuses
- 💬 Real-time chat using sockets
- 🎨 Unique color for each viewer in chat
- 👥 Following system
- 🚫 Blocking system
- 👢 Kicking participants from a stream in real-time
- 🎛️ Streamer / Creator Dashboard
- 🐢 Slow chat mode
- 🔒 Followers only chat mode
- 📴 Enable / Disable chat
- 🔽 Collapsible layout (hide sidebars, chat etc, theatre mode etc.)
- 📚 Sidebar following & recommendations tab
- 🏠 Home page recommending streams, sorted by live first
- 🔍 Search results page with a different layout
- 🔄 Syncing user information to our DB using Webhooks
- 📡 Syncing live status information to our DB using Webhooks
- 🤝 Community tab
- 🎨 Beautiful design
- ⚡ Blazing fast application
- 📄 SSR (Server-Side Rendering)
- 🗺️ Grouped routes & layouts
- 🗃️ MongoDB
- 🚀 Deployment

<!-- HOW TO RUN -->

### Prerequisites

**Node version 18.x.x**
**Yarn version 1.22.x**

### Start the app

Certainly, if you're working on a Node.js project and you have a development script, such as `yarn dev`, that you typically use to run your application during development, you can include that step in your workflow as well. Here's the updated order of commands:

1. **Clone this repository**:

   ```sh
   git clone git@github.com/Prakash-sa/twitch-clone.git
   ```

2. **Environment Variables Setup**:
   To rename the `.env.example` file to `.env` and add your environment-specific configuration, you can use the following command in a Unix-like shell (such as Linux or macOS):

   ```bash
   mv .env.example .env
   ```

   This command renames the `.env.example` file to `.env`.

   After renaming the file, you can open the `.env` file using a text editor and add your environment-specific configuration variables and their values. For example:

   ```
   DATABASE_URL=your_database_url_here
   API_KEY=your_api_key_here
   SECRET_KEY=your_secret_key_here
   ```

   Replace `"your_database_url_here"`, `"your_api_key_here"`, and `"your_secret_key_here"` with your actual configuration values. The `.env` file is commonly used to store sensitive or environment-specific configuration variables for your application.

3. **Install packages**

   ```shell
   yarn install
   ```

4. **Prisma Setup**:

   - Generate Prisma Client Code:

     ```bash
     npx prisma generate
     ```

   - Push Database Changes:

     ```bash
     npx prisma db push
     ```

   - Launch Prisma Studio: `optional`

     ```bash
     npx prisma studio
     ```

     Your `Prisma` database is accessible locally at the following address: [http://localhost:5555](http://localhost:5555)

5. **Run Your Application in Development Mode**:

   ```bash
   yarn dev
   ```

   Your `project` is accessible locally at the following address: [http://localhost:3000](http://localhost:3000)

### How to setup the initial project

1.  **Install Next JS**

    ```sh
    yarn create next-app --typescript --tailwind --eslint
    ```

2.  **Engine Locking configuration `optional`**

    - Create `.npmrc` file and add below the code

      ```sh
      engine-strict=true
      ```

    - Create `.nvmrc` file and add below the code

      ```sh
      lts/fermium
      ```

    - Add this configuration to your project `package.json`

      ```json
      "engines": {
         "node": ">=18.0.0",
         "yarn": ">=1.22.0",
         "npm": "please-use-yarn"
       }
      ```

3.  **Shadcn Ui Setup**
    - Initialize Shadcn ui
      ```bash
      npx shadcn-ui@latest init
      ```
    - How to use [Shadcn ui](https://ui.shadcn.com/) `optional`
      ```bash
      npx shadcn-ui@latest add button
      ```
    - Overwrite existing ui components `optional`
      ```bash
      npx shadcn-ui@latest add button --overwrite
      ```

## Contact

Prakash Saini - [sainiprakash525@gmail.com](mailto:sainiprakash525@gmail.com)
