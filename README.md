# My Personal Blog

A personal blog built with [Hugo Blox](https://hugoblox.com/) and hosted on [GitLab Pages](https://docs.gitlab.com/ee/user/project/pages/).

## Quick Start

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (v0.159+)
- [Go](https://golang.org/dl/)
- [Node.js](https://nodejs.org/) (for TailwindCSS)

### Local Development

```bash
# Install dependencies
npm install

# Start local server
hugo server --buildDrafts
```

Then visit [http://localhost:1313](http://localhost:1313).

### Build

```bash
hugo --gc --minify
```

## Deployment to GitLab Pages

The site is automatically deployed to GitLab Pages using the `.gitlab-ci.yml` configuration.

1. Push your code to GitLab:
   ```bash
   git remote add origin git@gitlab.com:<your-username>/<your-repo>.git
   git branch -M main
   git push -u origin main
   ```

2. GitLab CI/CD will automatically build and deploy your site.

3. Your site will be available at: `https://<your-username>.gitlab.io/<your-repo>/`

## Structure

```
├── config/_default/    # Hugo configuration
├── content/            # Your content (blog posts, pages, etc.)
├── assets/             # CSS, JS, and media files
├── layouts/            # Custom layouts (optional)
├── static/             # Static files
├── hugoblox.yaml       # Hugo Blox configuration
└── .gitlab-ci.yml      # GitLab CI/CD configuration
```

## License

This project is licensed under the [MIT License](LICENSE.md).
