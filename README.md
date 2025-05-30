# Custom CSS Framework

A lightweight, customizable CSS framework built with Sass that provides beautiful default styling for HTML elements and utility classes for rapid development.

## Team Members & Work Division

### **Leader**: David Muñoz Jensen - GitHub: [muoz0003](https://github.com/muoz0003)
**Responsibilities:**
- Project setup and repository management
- Sass compilation configuration (package.json, build scripts)
- Main entry point (`src/main.scss`)
- Variables system (`src/variables/_config.scss`, `src/variables/_colors.scss`)
- Base typography and headings (`src/base/_typography.scss`)
- Final integration and testing
- README documentation coordination
- Demo/example HTML file creation (`examples/index.html`)

### Chuhong Feng - GitHub: [philagoodday](https://github.com/philagoodday)
**Responsibilities:**
- Base HTML element styling:
  - Lists (`src/base/_lists.scss`)
  - Tables (`src/base/_tables.scss`)
  - Forms and inputs (`src/base/_forms.scss`)
- Utility classes for spacing:
  - Margin utilities (`src/utilities/_margin.scss`)
  - Padding utilities (`src/utilities/_padding.scss`)

### Solomon Tesfaye - GitHub: [tesf0059](https://github.com/tesf0059)
**Responsibilities:**
- Base HTML element styling:
  - Buttons (`src/base/_buttons.scss`)
  - Links and text elements (`src/base/_text.scss`)
- Utility classes for visual styling:
  - Color utilities (`src/utilities/_colors.scss`)
  - Border utilities (`src/utilities/_borders.scss`)
  - Font weight utilities (`src/utilities/_typography.scss`)

### Luz Helena Rodriguez - GitHub: [Rodr0288](https://github.com/Rodr0288)
**Responsibilities:**
- Base foundation styles:
  - CSS Reset/Normalize (`src/base/_reset.scss`)
  - Base layout styles (`src/base/_layout.scss`)
- Utility classes:
  - Font size utilities (`src/utilities/_font-sizes.scss`)
  - Display utilities (`src/utilities/_display.scss`)


## Features
-  Beautiful default styling for all HTML elements
-  Utility classes for rapid development
-  Sass-based with customizable variables
-  Responsive design principles
-  Lightweight and performant

## Installation

### Option 1: Download
Download the compiled CSS file from the `dist/` folder and include it in your HTML:

```html
<link rel="stylesheet" href="path/to/framework.css">
```

### Option 2: Build from Source
1. Clone the repository
2. Install dependencies: `npm install`
3. Build the framework: `npm run build`

## Usage

### Basic HTML Structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Project</title>
    <link rel="stylesheet" href="path/to/framework.css">
</head>
<body>
    <!-- Your content here -->
</body>
</html>
```

### Styled Elements
All standard HTML elements come with beautiful default styling:
- Headings (h1-h6)
- Paragraphs and text elements
- Lists (ul, ol, dl)
- Buttons and form elements
- Tables
- And more...

### Utility Classes

#### Colors
```html
<p class="text-primary">Primary text color</p>
<p class="text-secondary">Secondary text color</p>
<div class="bg-primary">Primary background</div>
```

#### Typography
```html
<p class="font-bold">Bold text</p>
<p class="font-light">Light text</p>
<p class="text-lg">Large text</p>
<p class="text-sm">Small text</p>
```

#### Spacing
```html
<div class="m-1">Margin small</div>
<div class="p-2">Padding medium</div>
<div class="mt-3">Margin top large</div>
```

#### Borders
```html
<div class="border">Default border</div>
<div class="border-rounded">Rounded border</div>
<div class="border-thick">Thick border</div>
```

## Customization

### Using Sass Variables
To customize the framework, modify the variables in `src/variables/_config.scss`:

```scss
// Colors
$primary-color: #007bff;
$secondary-color: #6c757d;
$success-color: #28a745;

// Typography
$font-family-base: 'Helvetica Neue', sans-serif;
$font-size-base: 1rem;
$line-height-base: 1.5;

// Spacing
$spacer: 1rem;
$spacers: (
  0: 0,
  1: $spacer * 0.25,
  2: $spacer * 0.5,
  3: $spacer,
  4: $spacer * 1.5,
  5: $spacer * 3
);
```

### Building Custom Version
1. Modify variables in `src/variables/_config.scss`
2. Run `npm run build` to compile your custom version
3. Use the generated CSS from `dist/framework.css`

## File Structure
```
src/
├── base/
│   ├── _reset.scss          # Luz Helena
│   ├── _typography.scss     # David
│   ├── _buttons.scss        # Solomon
│   ├── _forms.scss          # Chuhong
│   ├── _tables.scss         # Chuhong
│   ├── _lists.scss          # Chuhong
│   ├── _text.scss           # Solomon
│   └── _layout.scss         # Luz Helena
├── utilities/
│   ├── _colors.scss         # Solomon
│   ├── _typography.scss     # Solomon
│   ├── _font-sizes.scss     # Luz Helena
│   ├── _margin.scss         # Chuhong
│   ├── _padding.scss        # Chuhong
│   ├── _borders.scss        # Solomon
│   └── _display.scss        # Luz Helena
├── variables/
│   ├── _config.scss         # David
│   └── _colors.scss         # David
└── main.scss                # David

dist/
└── framework.css            # Compiled output

examples/
└── demo.html                # David
```

## Development

### Prerequisites
- Node.js and npm
- Sass compiler

### Setup
```bash
git clone <repository-url>
cd custom_css_framework
npm install
```

### Available Scripts
- `npm run build` - Compile Sass to CSS
- `npm run watch` - Watch for changes and auto-compile
- `npm run clean` - Remove compiled files

## Browser Support
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Contributing
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License
This project is licensed under the MIT License.

## Changelog
### v1.0.0
- Initial release
- Base HTML element styling
- Utility classes for common styling
- Sass variable system for customization