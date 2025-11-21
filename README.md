# Portfolio Website Template

A modern, responsive portfolio website template that can be easily customized for anyone's use. This single-page portfolio displays projects with images, descriptions, and links in a clean, professional layout.

## Development

This portfolio website was developed using **Cursor AI IDE**, an AI-powered code editor that significantly accelerated the development process. The AI assistant helped with generating responsive layouts, implementing dynamic content loading, creating flexible image galleries, and ensuring cross-browser compatibility.

The entire project is built with vanilla HTML, CSS, and JavaScript, no frameworks or build tools required, making it easy to deploy and customize.

## Features

- Fully responsive design for all devices
- Easy configuration through JSON and text files
- Support for PNG, GIF, and JPG images
- Automatic grid layouts for images
- Rich project descriptions with image annotations
- Optional GitHub repository links
- PDF export functionality
- No build process required

## Quick Setup

### Personalize Content

Edit `index.html` to update:
- Your name, title, and bio in the hero section
- Contact information (email, phone, location)
- Social media links

### Customize Styling

Modify the CSS in `index.html` to change colors, fonts, and layout. The default theme uses a dark background with purple/blue accents.

### Add Projects

1. Create a folder for each project in the `projects/` directory
2. Add your images (PNG, GIF, or JPG) to each project folder
3. Create a `description.txt` file with your project description
4. Update `projects/projects.json` with project details:

```json
[
    {
        "id": "project-folder-name",
        "title": "Project Title",
        "purpose": "Company or Personal Project",
        "githubLink": "https://github.com/username/repo",
        "images": ["image1.png", "image2.gif"]
    }
]
```

### Project Descriptions

In each project's `description.txt` file, write your main description followed by image-specific notes using letters (a., b., c., etc.) or the format "Image 1:", "Image 2:", etc.

## Project Structure

```
.
├── index.html
├── projects/
│   ├── projects.json
│   └── project-name/
│       ├── images...
│       └── description.txt
```

Feel free to use this portfolio template for your own projects!
