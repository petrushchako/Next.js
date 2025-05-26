# Phase 1: Setup and Introduction

### Step 1: Install Node.js (if not already installed)
Next.js requires Node.js (version 16.8 or newer).

#### Check if Node.js is installed
Open your terminal and run:

```bash
node -v
npm -v
```

If you get version numbers, you're good to go.

#### If Node.js is not installed

* Go to [https://nodejs.org/](https://nodejs.org/)
* Download the **LTS version**
* Install it with default options

This will also install **npm** (Node Package Manager), which you'll use to install dependencies.

<br>

### Step 2: Create a New Next.js App
We’ll use the official `create-next-app` command.

#### Run this in your terminal:
```bash
npx create-next-app@latest nextjs-advertising-site
```
It will prompt you with some questions:

| Prompt                              | Recommendation                                              |
| ----------------------------------- | ----------------------------------------------------------- |
| What is your project named?         | `nextjs-advertising-site`                                   |
| TypeScript with this project?       | **Yes** (recommended for long-term maintainability)         |
| Use ESLint?                         | Yes                                                         |
| Use Tailwind CSS?                   | Yes (we’ll use it for styling)                              |
| Use `src/` directory?               | Yes (cleaner structure)                                     |
| Use App Router?                     | **No** (we’ll stick to the **Pages Router** for simplicity) |
| Customize the default import alias? | No                                                          |

This creates a folder with all the files you need to start coding.

<br>

### Step 3: Explore Project Structure
Navigate into your project:
```bash
cd nextjs-advertising-site
```

Now open it in VS Code:
```bash
code .
```

<br>

Here's what you’ll see:

```
nextjs-advertising-site/
├── node_modules/          # dependencies
├── public/                # static assets (images, etc.)
├── src/
│   ├── pages/             # routing (index.tsx = home page)
│   └── styles/            # global and component styles
├── tailwind.config.js     # Tailwind setup
├── package.json           # project dependencies and scripts
```

<br>

### Step 4: Run the Development Server
Start the local server:
```bash
npm run dev
```
Visit your site at [http://localhost:3000](http://localhost:3000)
You should see the default Next.js welcome page.

<br>

### Step 5: Initialize Git Repo
Inside the project directory:
```bash
git init
git add .
git commit -m "Initial Next.js setup"
```

You can also push this to GitHub if desired:
```bash
gh repo create nextjs-advertising-site --public --source=. --remote=origin
git push -u origin main
```
