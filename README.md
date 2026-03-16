<div align="center">

# create-frontend-app

🚀 **The Ultimate Frontend Project Scaffolding Tool**

[![npm version](https://img.shields.io/npm/v/create-frontend-app.svg?style=flat-square)](https://www.npmjs.com/package/create-frontend-app)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
[![Node Version](https://img.shields.io/badge/node-%3E%3D16.0.0-brightgreen?style=flat-square)](https://nodejs.org)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://github.com/gandharrdotexe/create-frontend-app/pulls)

*Stop wasting time on boilerplate. Start building features.*

[Quick Start](#-quick-start) • [Features](#-features) • [Templates](#-templates) • [Documentation](#-documentation) • [Examples](#-examples)

</div>

---

## 📑 Table of Contents

- [Why create-frontend-app?](#-why-create-frontend-app)
- [Features](#-features)
- [Quick Start](#-quick-start)
- [Templates](#-templates)
- [Usage](#-usage)
- [Comparison](#-comparison)
- [Supported Technologies](#-supported-technologies)
- [Project Structure](#-project-structure)
- [Examples](#-examples)
- [Configuration](#️-configuration)
- [FAQ](#-faq)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)
- [Support & Community](#-support--community)

---

## 🎯 Why create-frontend-app?

Setting up a modern frontend project shouldn't take hours. **create-frontend-app** gives you a production-ready project in under 2 minutes with:

- ✅ Your choice of framework (React, Next.js, Vue, and more)
- ✅ TypeScript configured correctly
- ✅ Tailwind CSS or your preferred styling solution
- ✅ UI components ready to use (shadcn/ui, MUI, etc.)
- ✅ Linting, formatting, and testing set up
- ✅ Git, Docker, and CI/CD configured
- ✅ Best practices baked in

**No more config files. No more dependency hell. Just code.**

## ✨ Features

<table>
<tr>
<td width="50%">

### 🎨 **Frontend Powerhouse**
- 🎯 Interactive CLI with smart prompts
- ⚡ 7 frameworks supported
- 🎨 6 CSS solutions
- 🧩 7+ UI component libraries
- 📦 Works with npm, yarn, pnpm, bun

</td>
<td width="50%">

### 🛠️ **Developer Experience**
- 🔧 TypeScript ready
- ✅ ESLint & Prettier configured
- 🧪 Testing setup (Vitest/Playwright)
- 🐳 Docker containerization
- 🤖 GitHub Actions CI/CD

</td>
</tr>
</table>


## 🚀 Quick Start

### One Command to Rule Them All

```bash
npx create-frontend-app my-app
```

That's it! In under 2 minutes, you'll have a fully configured project ready to go.

<details>
<summary><b>📦 Using Different Package Managers</b></summary>

```bash
# npm (recommended)
npm create frontend-app my-app

# yarn
yarn create frontend-app my-app

# pnpm
pnpm create frontend-app my-app

# bun
bun create frontend-app my-app
```
</details>

### 🎬 What Happens Next?

After running the command, you'll see:

```
┌─────────────────────────────────────────┐
│  Create Frontend App v1.0.0             │
└─────────────────────────────────────────┘

? Project name: my-app
? Which framework would you like to use? React (Vite)
? Would you like to use TypeScript? Yes
? Which CSS solution would you like to use? Tailwind CSS
? Would you like to add a UI component library? shadcn/ui
? Select additional tools: ESLint, Prettier
? Which package manager would you like to use? npm

✓ Created project structure
✓ Installing dependencies...
✓ Initializing git repository

✨ Success! Created my-app

Next steps:
  cd my-app
  npm run dev

Happy coding! 🚀
```

Then just:

```bash
cd my-app
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) and start building! 🎉


## 🎁 Templates

Skip the questions and get started instantly with our battle-tested templates:

```bash
npx create-frontend-app my-app --template <template-name>
```

### Available Templates

| Template | Description | Best For |
|----------|-------------|----------|
| `minimal` | React + Vite, JavaScript only | Learning, simple projects |
| `react-ts-tailwind` | React + TypeScript + Tailwind | Most React projects |
| `react-shadcn` | React + TS + Tailwind + shadcn/ui | Modern web apps |
| `nextjs-full` | Next.js + TS + Tailwind + Tools | SEO-focused sites, full-stack apps |
| `vue-ts` | Vue 3 + TypeScript + Tailwind | Vue enthusiasts |
| `enterprise` | **Everything included** | Production apps, teams |

<details>
<summary><b>🏢 Enterprise Template Details</b></summary>

The `enterprise` template includes:
- ✅ Next.js 14 with App Router
- ✅ TypeScript with strict mode
- ✅ Tailwind CSS + shadcn/ui
- ✅ ESLint + Prettier
- ✅ Husky + lint-staged (pre-commit hooks)
- ✅ Vitest (unit tests) + Playwright (E2E)
- ✅ Docker multi-stage build
- ✅ GitHub Actions CI/CD
- ✅ pnpm for faster installs

Perfect for teams that want everything configured from day one.
</details>

## 📖 Usage

### 🎯 Interactive Mode (Recommended for First-Timers)

Simply run the command and answer the prompts:

```bash
npx create-frontend-app my-app
```

**You'll be asked about:**

| Step | Question | Options |
|------|----------|---------|
| 1️⃣ | Project name | Any valid npm package name |
| 2️⃣ | Framework | React, Next.js, Vue, Nuxt, SvelteKit, Solid, Vanilla |
| 3️⃣ | TypeScript? | Yes / No |
| 4️⃣ | CSS solution | Tailwind, Sass, Styled Components, Emotion, CSS Modules, Vanilla |
| 5️⃣ | UI library | shadcn/ui, MUI, Ant Design, Chakra UI, DaisyUI, Vuetify, PrimeVue, None |
| 6️⃣ | Tools | ESLint, Prettier, Husky, Vitest, Playwright, Docker, GitHub Actions |
| 7️⃣ | Package manager | npm, yarn, pnpm, bun |

### ⚡ Quick Mode (Templates)

Skip all questions with a template:

```bash
npx create-frontend-app my-app --template <template-name>
```

### 🔧 Command Line Options

```bash
create-frontend-app [project-name] [options]
```

**Available Options:**

| Option | Description | Example |
|--------|-------------|---------|
| `-t, --template <name>` | Use predefined template | `--template react-shadcn` |
| `--skip-git` | Skip git initialization | `--skip-git` |
| `--skip-install` | Skip installing dependencies | `--skip-install` |
| `-V, --version` | Show version number | `-V` |
| `-h, --help` | Display help information | `-h` |

**Examples:**

```bash
# Use template + skip git
npx create-frontend-app my-app --template minimal --skip-git

# Custom name + skip install (install manually later)
npx create-frontend-app cool-project --skip-install

# Get help
npx create-frontend-app --help
```

## 🆚 Comparison

### vs Create React App

| Feature | create-frontend-app | Create React App |
|---------|-------------------|------------------|
| Build Tool | Vite (⚡ fast) | Webpack (slower) |
| Frameworks | 7 supported | React only |
| TypeScript | Optional | Optional |
| UI Libraries | 7+ pre-configured | Manual setup |
| Testing | Vitest/Playwright | Jest/RTL |
| Maintenance | ✅ Active | ⚠️ Deprecated |
| Bundle Size | Smaller | Larger |
| HMR Speed | <100ms | 1-3s |

### vs Manual Setup

| Task | Manual | create-frontend-app |
|------|--------|-------------------|
| Initial setup | 2-4 hours | < 2 minutes |
| Config files | Write yourself | Auto-generated |
| Dependencies | Research & install | Pre-selected |
| Best practices | Study docs | Built-in |
| TypeScript | Complex setup | One checkbox |
| Testing | Multiple tools to learn | Pre-configured |

## 🎯 Supported Technologies

### Frameworks

- ⚛️ **React** (with Vite)
- ⚡ **Next.js** (App Router)
- 💚 **Vue 3** (with Vite)
- 🔷 **Nuxt 3**
- 🔥 **SvelteKit**
- 🟦 **Solid** (with Vite)
- 📝 **Vanilla JS** (with Vite)

### CSS Solutions

- 🎨 **Tailwind CSS** - Utility-first CSS framework
- 📦 **CSS Modules** - Scoped CSS
- 🎭 **Sass/SCSS** - CSS preprocessor
- 💅 **Styled Components** - CSS-in-JS
- 😶 **Emotion** - CSS-in-JS
- 📄 **Vanilla CSS** - Plain CSS

### UI Component Libraries

- 🎨 **shadcn/ui** - Re-usable components (React + Tailwind)
- 🎯 **Material-UI** - React components
- 🐜 **Ant Design** - Enterprise-class UI
- ⚡ **Chakra UI** - Accessible component library
- 🌼 **DaisyUI** - Tailwind CSS components
- 💎 **Vuetify** - Vue Material Design
- 🎭 **PrimeVue** - Vue UI suite

### Development Tools

- ✅ **ESLint** - Code linting
- 🎨 **Prettier** - Code formatting
- 🐶 **Husky** - Git hooks
- ⚡ **Vitest** - Unit testing
- 🎭 **Playwright** - E2E testing
- 🐳 **Docker** - Containerization
- 🤖 **GitHub Actions** - CI/CD workflows

## 📁 Project Structure

Generated projects follow best practices:

```
my-app/
├── .github/
│   └── workflows/          # CI/CD workflows
├── .husky/                 # Git hooks
├── public/                 # Static assets
├── src/
│   ├── assets/            # Images, fonts, etc.
│   ├── components/        # React/Vue components
│   │   └── ui/           # UI library components
│   ├── lib/              # Utility functions
│   ├── styles/           # Global styles
│   ├── App.tsx           # Main component
│   └── main.tsx          # Entry point
├── tests/                 # Test files
├── .env.example          # Environment variables template
├── .eslintrc.json        # ESLint configuration
├── .gitignore            # Git ignore rules
├── .prettierrc           # Prettier configuration
├── package.json          # Dependencies and scripts
├── README.md             # Project documentation
├── tailwind.config.js    # Tailwind configuration
├── tsconfig.json         # TypeScript configuration
└── vite.config.ts        # Vite configuration
```

## 🎓 Examples

### 🌟 Real-World Use Cases

<details>
<summary><b>🛍️ E-commerce Product Page</b></summary>

```bash
npx create-frontend-app shop-frontend --template react-shadcn
cd shop-frontend
npm run dev
```

**What you get:**
- React with TypeScript
- Tailwind CSS for styling
- shadcn/ui components (cards, buttons, dialogs)
- Pre-configured for building product catalogs

**Next steps:**
- Add product components in `src/components/`
- Create shopping cart logic
- Integrate with your API
</details>

<details>
<summary><b>📱 SaaS Landing Page</b></summary>

```bash
npx create-frontend-app saas-landing --template nextjs-full
cd saas-landing
npm run dev
```

**What you get:**
- Next.js for SEO optimization
- TypeScript for type safety
- Tailwind CSS for rapid styling
- ESLint & Prettier for code quality

**Perfect for:**
- Marketing websites
- Product landing pages
- Blog with static generation
</details>

<details>
<summary><b>📊 Admin Dashboard</b></summary>

```bash
npx create-frontend-app admin-panel --template enterprise
cd admin-panel
npm run dev
```

**What you get:**
- Next.js with App Router
- shadcn/ui with data tables, forms
- Vitest for unit tests
- Playwright for E2E tests
- Docker for deployment
- CI/CD pipeline ready

**Ideal for:**
- Internal tools
- Analytics dashboards
- Admin panels
</details>

<details>
<summary><b>🎨 Portfolio Website</b></summary>

```bash
npx create-frontend-app portfolio
# Choose: React (Vite), TypeScript: Yes, CSS: Tailwind, UI: shadcn/ui
cd portfolio
npm run dev
```

**What you get:**
- Fast Vite development server
- Beautiful shadcn/ui components
- Responsive design ready
- TypeScript for maintainability

**Build:**
- About page
- Projects showcase
- Contact form
- Blog section
</details>

<details>
<summary><b>🎮 Interactive Web App</b></summary>

```bash
npx create-frontend-app game-app
# Choose: React (Vite), TypeScript: Yes, CSS: Styled Components
cd game-app
npm run dev
```

**What you get:**
- React for interactive UI
- Styled Components for dynamic styling
- TypeScript for game logic
- Fast HMR for quick iterations

**Great for:**
- Browser games
- Interactive experiences
- Animation-heavy apps
</details>

### 📝 Step-by-Step Walkthroughs

#### Create a Blog with Next.js

```bash
# 1. Create project
npx create-frontend-app my-blog --template nextjs-full

# 2. Navigate to project
cd my-blog

# 3. Start development
npm run dev

# 4. Open browser
# Visit http://localhost:3000

# 5. Start building
# Edit src/app/page.tsx
# Add blog posts in src/app/blog/
```

#### Create a Vue Dashboard

```bash
# 1. Create project with Vue
npx create-frontend-app dashboard --template vue-ts

# 2. Install chart library
cd dashboard
npm install chart.js vue-chartjs

# 3. Start development
npm run dev

# 4. Build components
# Create charts in src/components/
# Add routing with Vue Router if needed
```

### 🔄 Migration Examples

<details>
<summary><b>Moving from Create React App?</b></summary>

```bash
# Create new project with Vite (much faster!)
npx create-frontend-app my-app --template react-ts-tailwind

# Copy your source files
cp -r old-project/src/* my-app/src/

# Install any additional dependencies
cd my-app
npm install axios react-router-dom

# Update imports if needed (Vite uses ES modules)
# Start dev server
npm run dev
```

**Benefits:**
- ⚡ 10-100x faster HMR
- 📦 Smaller bundle sizes
- 🔧 Modern build tooling
</details>

## ⚙️ Configuration

All generated projects come with sensible defaults, but everything is customizable!

### 🔍 ESLint Configuration

Projects with ESLint include:

```json
// .eslintrc.json
{
  "env": { "browser": true, "es2021": true, "node": true },
  "extends": [
    "eslint:recommended",
    "plugin:react/recommended",        // For React projects
    "plugin:@typescript-eslint/recommended"  // For TypeScript
  ],
  "rules": {
    "react/react-in-jsx-scope": "off"  // Not needed in React 17+
  }
}
```

**Customize it:**
```bash
# Add your own rules in .eslintrc.json
{
  "rules": {
    "no-console": "warn",
    "prefer-const": "error"
  }
}
```

### 🎨 Prettier Configuration

Default Prettier setup:

```json
// .prettierrc
{
  "semi": true,
  "trailingComma": "es5",
  "singleQuote": true,
  "printWidth": 80,
  "tabWidth": 2,
  "plugins": ["prettier-plugin-tailwindcss"]  // If Tailwind selected
}
```

**Customize it:**
```json
{
  "semi": false,        // Remove semicolons
  "singleQuote": false, // Use double quotes
  "printWidth": 100     // Longer lines
}
```

### 📘 TypeScript Configuration

TypeScript projects include strict mode:

```json
// tsconfig.json
{
  "compilerOptions": {
    "target": "ES2020",
    "strict": true,
    "noUnusedLocals": true,
    "noUnusedParameters": true,
    "jsx": "react-jsx",  // For React
    "paths": {
      "@/*": ["./src/*"]  // For shadcn/ui
    }
  }
}
```

**Common customizations:**
```json
{
  "compilerOptions": {
    "strict": false,           // Disable strict mode
    "skipLibCheck": true,      // Faster builds
    "baseUrl": ".",            // Absolute imports
    "paths": {
      "@components/*": ["src/components/*"],
      "@utils/*": ["src/utils/*"]
    }
  }
}
```

### 🎨 Tailwind CSS Configuration

Tailwind projects include:

```js
// tailwind.config.js
export default {
  content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {},  // Customize your theme here
  },
  plugins: [],
}
```

**Extend with custom colors:**
```js
theme: {
  extend: {
    colors: {
      primary: '#3b82f6',
      secondary: '#8b5cf6',
    },
    fontFamily: {
      sans: ['Inter', 'sans-serif'],
    },
  },
}
```

### 🧪 Vitest Configuration

Testing projects include:

```ts
// vitest.config.ts
export default defineConfig({
  test: {
    globals: true,
    environment: 'jsdom',
    setupFiles: './tests/setup.ts',
  },
})
```

**Add coverage thresholds:**
```ts
test: {
  coverage: {
    provider: 'v8',
    reporter: ['text', 'html'],
    lines: 80,
    functions: 80,
    branches: 80,
  },
}
```

### 🐶 Husky Configuration

Git hooks are configured with:

```bash
# .husky/pre-commit
npx lint-staged
```

```json
// .lintstagedrc.json
{
  "*.{js,jsx,ts,tsx}": ["eslint --fix", "prettier --write"],
  "*.{json,css,md}": ["prettier --write"]
}
```

**Add custom hooks:**
```bash
npx husky add .husky/pre-push "npm test"
```

### 🔧 VS Code Settings (Recommended)

Create `.vscode/settings.json`:

```json
{
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "typescript.tsdk": "node_modules/typescript/lib"
}
```

## ❓ FAQ

<details>
<summary><b>Can I use this for production projects?</b></summary>

Absolutely! All generated projects follow industry best practices and are production-ready. Many teams use this CLI to standardize their project setup.
</details>

<details>
<summary><b>How do I add more components from shadcn/ui?</b></summary>

After creating your project with shadcn/ui, you can add components using:

```bash
npx shadcn-ui@latest add button
npx shadcn-ui@latest add card
npx shadcn-ui@latest add dialog
```

See [shadcn/ui documentation](https://ui.shadcn.com/docs) for all available components.
</details>

<details>
<summary><b>Can I customize the templates?</b></summary>

Yes! After generating a project, you can modify it however you like. For creating custom templates programmatically, check out our [SETUP.md](SETUP.md) guide.
</details>

<details>
<summary><b>Which package manager should I use?</b></summary>

- **npm**: Most compatible, comes with Node.js
- **pnpm**: Fastest, most disk-efficient
- **yarn**: Popular, good monorepo support
- **bun**: Newest, extremely fast

The CLI auto-detects your preference!
</details>

<details>
<summary><b>Does this work on Windows?</b></summary>

Yes! The CLI works on Windows, macOS, and Linux. On Windows, we recommend using PowerShell or Windows Terminal.
</details>

<details>
<summary><b>Can I skip TypeScript?</b></summary>

Yes! When prompted, just select "No" for TypeScript. All templates except enterprise mode support JavaScript.
</details>

<details>
<summary><b>How do I update dependencies later?</b></summary>

Use your package manager's update commands:

```bash
npm update        # Updates to latest minor/patch versions
npm outdated      # Check for newer versions
npx npm-check-updates -u  # Update to latest major versions
```
</details>

## 🐛 Troubleshooting

### Command not found

```bash
# If you get "create-frontend-app: command not found"
# Make sure you're using npx:
npx create-frontend-app my-app

# Or install globally:
npm install -g create-frontend-app
```

### Permission errors

```bash
# On Linux/Mac, if you get permission errors:
sudo chown -R $USER /usr/local/lib/node_modules

# Or use a version manager like nvm (recommended)
```

### Git initialization fails

```bash
# Make sure git is installed:
git --version

# If not installed, install git first
# Or skip git initialization:
npx create-frontend-app my-app --skip-git
```

### Dependencies installation fails

```bash
# Clear npm cache and try again:
npm cache clean --force
npx create-frontend-app my-app

# Or skip installation and do it manually:
npx create-frontend-app my-app --skip-install
cd my-app
npm install
```

### Port already in use

```bash
# If dev server won't start (port 5173 in use):
# Kill the process on that port or use a different port:
npm run dev -- --port 3000
```

### Module not found errors

```bash
# Delete node_modules and reinstall:
rm -rf node_modules package-lock.json
npm install
```

<details>
<summary><b>🔍 Still having issues?</b></summary>

1. Make sure you're using Node.js 16 or higher: `node --version`
2. Update npm to the latest version: `npm install -g npm@latest`
3. Try running with verbose logging: `npx create-frontend-app my-app --verbose`
4. Check our [GitHub Issues](https://github.com/gandharrdotexe/create-frontend-app/issues)
5. Create a new issue with your error message and system info
</details>

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by [create-react-app](https://github.com/facebook/create-react-app)
- Built with [Commander.js](https://github.com/tj/commander.js/)
- Uses [Inquirer.js](https://github.com/SBoudrias/Inquirer.js) for prompts
- Styling with [Chalk](https://github.com/chalk/chalk)

## 📧 Support & Community

<div align="center">

### Get Help

[![Documentation](https://img.shields.io/badge/docs-read%20now-blue?style=for-the-badge)](https://github.com/gandharrdotexe/create-frontend-app)
[![Issues](https://img.shields.io/badge/issues-report%20bug-red?style=for-the-badge)](https://github.com/gandharrdotexe/create-frontend-app/issues)
[![Discussions](https://img.shields.io/badge/discussions-join%20chat-green?style=for-the-badge)](https://github.com/gandharrdotexe/create-frontend-app/discussions)

</div>

### 📚 Resources

- 📖 [Full Documentation](https://github.com/gandharrdotexe/create-frontend-app)
- 🚀 [Quick Start Guide](QUICKSTART.md)
- 🔧 [Development Setup](SETUP.md)
- ✨ [Feature List](FEATURES.md)
- 🐛 [Issue Tracker](https://github.com/gandharrdotexe/create-frontend-app/issues)
- 💬 [Discussions Forum](https://github.com/gandharrdotexe/create-frontend-app/discussions)

### 🌟 Show Your Support

If this project helped you, please consider:

- ⭐ Starring the repo
- 🐦 Sharing on Twitter
- 📝 Writing a blog post
- 🗣️ Telling your colleagues

## 🗺️ Roadmap

### Coming Soon
- [ ] **Remix** framework support
- [ ] **Astro** framework support
- [ ] Custom template creation tool
- [ ] Plugin system for extensions

### Future Plans
- [ ] Monorepo support (Turborepo, Nx)
- [ ] Backend scaffolding options
- [ ] Database integration wizards
- [ ] VS Code extension
- [ ] GUI desktop app
- [ ] Configuration presets (save & reuse)
- [ ] Interactive upgrade command

Want to help? Check our [Contributing Guide](#-contributing)!

## 📊 Stats

<div align="center">

![GitHub stars](https://img.shields.io/github/stars/gandharrdotexe/create-frontend-app?style=social)
![npm downloads](https://img.shields.io/npm/dm/create-frontend-app?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/gandharrdotexe/create-frontend-app?style=flat-square)

</div>

## 💝 Sponsors

This project is made possible by our amazing sponsors and contributors!

<!-- Add sponsors here when available -->

---

<div align="center">

**Made with ❤️ by developers, for developers**

[⬆ Back to Top](#create-frontend-app)

*Happy coding! 🚀*

</div>
