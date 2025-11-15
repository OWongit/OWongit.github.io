# Projects Folder Structure

Each project should be in its own folder within the `projects/` directory.

## Folder Structure

```
projects/
├── projects.json          # Manifest file listing all projects
├── project1/
│   ├── image1.png
│   ├── image2.png
│   ├── image3.png
│   ├── image4.png
│   └── description.txt
└── project2/
    ├── image1.png
    ├── image2.png
    ├── image3.png
    ├── image4.png
    ├── image5.png
    └── description.txt
```

## projects.json Format

Edit `projects.json` to add or modify projects:

```json
[
    {
        "id": "project1",
        "title": "Project 1: Example Engineering Project",
        "githubLink": "https://github.com/username/repo",
        "images": [
            "Image1.png",
            "image2.png",
            "my-screenshot.png",
            "photo.jpg"
        ]
    }
]
```

- `id`: Folder name (must match the folder name)
- `title`: Display title for the project
- `githubLink`: Optional GitHub repository link
- `images`: Array of image filenames (in order of display)

**Note:** You can also use the old format with `imageCount` (for numbered images like `image1.png`, `image2.png`, etc.), but specifying filenames directly gives you more control.

## Image Files

- You can use any filename for your images (e.g., `Image1.png`, `screenshot.png`, `photo.jpg`)
- List the exact filenames in the `images` array in `projects.json` in the order you want them displayed
- Images are automatically arranged in a grid:
  - 4 images = 2x2 grid
  - 5 images = 3 on top row, 2 on bottom row
  - Other counts are automatically formatted

## description.txt Format

The description file should contain:
1. Overall project description (one or more paragraphs)
2. Image descriptions (optional, one per image)

Example:

```
This is a comprehensive engineering project that demonstrates various technical skills and problem-solving abilities. The project involved multiple phases including design, development, testing, and deployment.

a. Initial design and architecture overview showing the system structure
b. Implementation phase demonstrating core functionality
c. Final testing and validation results
d. Deployment and performance metrics
```

- Lines starting with "a:", "a.", "b:", "b.", "c:", "c.", etc. will be displayed as headings with descriptions below
- You can also use the old format "Image 1:", "Image 2:", etc. (it will be converted to letters automatically)
- All other text is treated as the main project description
- Text appears after the images on the webpage
- Images are automatically labeled with lowercase letters (a, b, c, d, etc.) in the top-left corner

