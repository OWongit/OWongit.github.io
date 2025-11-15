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
        "imageCount": 4
    }
]
```

- `id`: Folder name (must match the folder name)
- `title`: Display title for the project
- `githubLink`: Optional GitHub repository link
- `imageCount`: Number of images (2-5 recommended, but any number works)

## Image Files

- Name images as `image1.png`, `image2.png`, `image3.png`, etc.
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

Image 1: Initial design and architecture overview showing the system structure
Image 2: Implementation phase demonstrating core functionality
Image 3: Final testing and validation results
Image 4: Deployment and performance metrics
```

- Lines starting with "Image X:" will be displayed as headings with descriptions below
- All other text is treated as the main project description
- Text appears after the images on the webpage

