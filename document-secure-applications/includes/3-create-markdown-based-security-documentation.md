Markdown is a versatile and widely-used language for creating documentation in code repositories. By adhering to security best practices, you can ensure that your documentation remains both accessible and secure.

## Use secure markdown practices
When working with Markdown files, it’s essential to follow security guidelines to protect sensitive information and maintain the integrity of your documentation.

- **Secret management:** Avoid including sensitive information such as API keys or passwords directly in Markdown files. Instead, use environment variables or secret management tools.
- **Access control:** Ensure that your repository permissions are configured correctly to restrict unauthorized access to Markdown files.
- **Link validation:** Use tools like Visual Studio Code’s link validation feature to check for broken or insecure links in your Markdown files.

:::image type="content" source="../media/theme-light.svg" alt-text="A warning shown in the editor when linking to a file that does not exist":::

> [!NOTE]
> Enable link validation in Visual Studio Code by setting `"markdown.validate.enabled": true` to catch common mistakes like linking to headers that were renamed or files that no longer exist.

## Enhance markdown documentation with advanced features
Markdown supports various advanced formatting options that can improve the readability and functionality of your documentation.

- **Tables:** Organize information using tables to present data clearly. For example:

   ```markdown
   | Rank | Languages |
   |-----:|-----------|
   |     1| JavaScript|
   |     2| Python    |
   |     3| SQL       |
   ```

- **Collapsed sections:** Use `<details>` tags to create expandable sections for lengthy content.

   ```html
   <details>
   <summary>My top languages</summary>

   | Rank | Languages |
   |-----:|-----------|
   |     1| JavaScript|
   |     2| Python    |
   |     3| SQL       |

   </details>
   ```

- **Responsive images:** Add images that adapt to light or dark mode using the `<picture>` element.

   ```html
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="dark-mode-image.png">
     <source media="(prefers-color-scheme: light)" srcset="light-mode-image.png">
     <img alt="Description of image" src="default-image.png">
   </picture>
   ```

## Secure markdown preview and extensions
Visual Studio Code provides features to enhance Markdown editing while maintaining security.

- **Preview security:** Restrict content displayed in the Markdown preview to trusted sources. Use the strict security setting to disable script execution and block insecure content.
- **Extensions:** Install extensions like spell checkers and Markdown linters to improve the quality of your documentation.

> [!TIP]
> Use the [Doc Writer profile template](https://code.visualstudio.com/docs/configure/profiles#_doc-writer-profile-template) in Visual Studio Code to quickly set up useful extensions and settings for Markdown editing.

By following these practices, you can create secure and effective Markdown-based documentation for your code repositories.