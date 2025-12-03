# Quickstart Guide: AI Driven Development Book Documentation (Docusaurus)

This guide provides instructions to quickly set up and run the AI Driven Development Book documentation site locally using Docusaurus.

## Prerequisites

Ensure you have the following installed on your system:

-   **Node.js** (LTS version recommended, e.g., 18.x or 20.x)
-   **npm** or **Yarn** (npm comes with Node.js, Yarn can be installed separately)

## 1. Clone the Repository (if you haven't already)

If you haven't cloned the repository containing this documentation project, do so first:

```bash
git clone [repository-url]
cd ai-book/ai-dev-book # Or wherever your project root is
```

## 2. Install Dependencies

Navigate to the root of your Docusaurus project (where `package.json` is located, which will be the project root for this documentation setup) and install the required Node.js packages:

```bash
npm install
# OR
yarn install
```

## 3. Start the Development Server

Once dependencies are installed, you can start the local development server. This will open the documentation site in your browser, and it will automatically reload upon content changes.

```bash
npm start
# OR
yarn start
```

By default, the site will be available at `http://localhost:3000/`.

## 4. Build the Static Site

To generate a static build of the documentation site (e.g., for deployment), run the build command:

```bash
npm run build
# OR
yarn build
```

The static assets will be generated in the `build/` directory (or a configurable output directory). You can then serve these static files using any web server.

## 5. Adding New Content

-   Markdown files for new documentation pages should be placed within the `docs/` directory, following the chapter structure defined in `data-model.md` and configured in `docusaurus.config.js`.
-   Docusaurus uses front matter (YAML at the top of a Markdown file) for metadata like `title`, `sidebar_position`, etc. Consult the Docusaurus documentation for more details on front matter and content organization.

## Troubleshooting

-   If you encounter issues, ensure Node.js and npm/Yarn are correctly installed and updated.
-   Refer to the official Docusaurus documentation for in-depth troubleshooting and advanced configurations.