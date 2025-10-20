# Blog System - EZERV Solutions

## How It Works

The blog system automatically fetches and displays blog posts from this `blogs` folder using the GitHub API.

## Adding New Blog Posts

1. **Create a new HTML file** in this `blogs` folder
2. **Name your file** using this format: `YYYY-MM-DD-blog-title.html`
   - Example: `2025-01-20-introduction-to-devops.html`
   - The date will be automatically extracted and displayed
   - Hyphens and underscores in the filename will be converted to spaces in the title

3. **Use the template** provided in `2025-01-15-cloud-migration-best-practices.html` as a reference

4. **Commit and push** your new blog HTML file to GitHub

5. The blog will **automatically appear** on the blogs page!

## Blog File Structure

Each blog HTML file should include:
- Standard header with navigation (copy from the sample)
- Blog post content with proper headings and formatting
- Author information
- Footer

## Important Notes

- Make sure to update the navigation links in your blog posts (they use `../` to go back to parent directory)
- The blog listing page fetches files from: `https://api.github.com/repos/ezervindia/ezerv3/contents/blogs`
- If you change your GitHub username or repository name, update the configuration in `blogs.html`:
  ```javascript
  const GITHUB_USER = 'ezervindia'; // Your GitHub username
  const GITHUB_REPO = 'ezerv3'; // Your repository name
  ```

## Sample Blog Post

See `2025-01-15-cloud-migration-best-practices.html` for a complete example of a blog post.

## Styling

All blog posts use:
- TailwindCSS for styling
- Feather Icons for icons
- Responsive design that works on all devices

Happy blogging! 🚀
