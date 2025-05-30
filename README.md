# Aesthetic CSS Framework

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
- Demo/example HTML file creation (`examples/demo.html`)

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
- Beautiful default styling for all HTML elements
- Utility classes for rapid development
- Sass-based with customizable variables
- Responsive design principles
- Lightweight and performant

## Installation

### Option 1: Download
Download the compiled CSS file from the `dist/` folder and include it in your HTML:

```html
<link rel="stylesheet" href="path/to/aesthetic.css">
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
    <link rel="stylesheet" href="path/to/aesthetic.css">
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
<p class="text-success">Success text color</p>
<p class="text-danger">Danger text color</p>
<div class="bg-primary">Primary background</div>
<div class="bg-secondary">Secondary background</div>
```

#### Typography
```html
<p class="font-bold">Bold text</p>
<p class="font-normal">Normal text</p>
<p class="font-light">Light text</p>
<p class="text-lg">Large text</p>
<p class="text-md">Medium text</p>
<p class="text-sm">Small text</p>
<p class="text-xs">Extra small text</p>
```

#### Spacing
```html
<!-- Margin classes -->
<div class="m-0">No margin</div>
<div class="m-1">Small margin</div>
<div class="m-2">Medium margin</div>
<div class="m-3">Large margin</div>
<div class="mt-2">Margin top</div>
<div class="mb-2">Margin bottom</div>
<div class="ml-2">Margin left</div>
<div class="mr-2">Margin right</div>

<!-- Padding classes -->
<div class="p-0">No padding</div>
<div class="p-1">Small padding</div>
<div class="p-2">Medium padding</div>
<div class="p-3">Large padding</div>
<div class="pt-2">Padding top</div>
<div class="pb-2">Padding bottom</div>
<div class="pl-2">Padding left</div>
<div class="pr-2">Padding right</div>
```

#### Borders
```html
<div class="border">Default border</div>
<div class="border-rounded">Rounded border</div>
<div class="border-thick">Thick border</div>
<div class="border-primary">Primary color border</div>
<div class="border-none">No border</div>
```

#### Display
```html
<div class="d-block">Display block</div>
<div class="d-inline">Display inline</div>
<div class="d-inline-block">Display inline-block</div>
<div class="d-flex">Display flex</div>
<div class="d-none">Display none</div>
```

## Customization

### Using Sass Variables
To customize the framework, modify the variables in `src/variables/_config.scss`:

```scss
// Colors
$primary-color: #007bff;
$secondary-color: #6c757d;
$success-color: #28a745;
$danger-color: #dc3545;
$warning-color: #ffc107;
$info-color: #17a2b8;

// Typography
$font-family-base: 'Helvetica Neue', Arial, sans-serif;
$font-size-base: 1rem;
$line-height-base: 1.5;

// Font weights
$font-weight-light: 300;
$font-weight-normal: 400;
$font-weight-bold: 700;

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

// Borders
$border-width: 1px;
$border-radius: 0.25rem;
$border-color: #dee2e6;
```

### Building Custom Version
1. Modify variables in `src/variables/_config.scss`
2. Run `npm run build` to compile your custom version
3. Use the generated CSS from `dist/aesthetic.css`

## File Structure
```
aesthetic_css_framework/
├── src/
│   ├── base/
│   │   ├── _reset.scss          # Luz Helena
│   │   ├── _typography.scss     # David - Base typography styling for HTML elements
│   │   ├── _buttons.scss        # Solomon
│   │   ├── _forms.scss          # Chuhong
│   │   ├── _tables.scss         # Chuhong
│   │   ├── _lists.scss          # Chuhong
│   │   ├── _text.scss           # Solomon
│   │   └── _layout.scss         # Luz Helena
│   ├── utilities/
│   │   ├── _colors.scss         # Solomon
│   │   ├── _typography.scss     # Solomon - Typography utilities for font weights and text styling
│   │   ├── _font-sizes.scss     # Luz Helena
│   │   ├── _margin.scss         # Chuhong
│   │   ├── _padding.scss        # Chuhong
│   │   ├── _borders.scss        # Solomon
│   │   └── _display.scss        # Luz Helena
│   ├── variables/
│   │   ├── _config.scss         # David - Configuration variables
│   │   └── _colors.scss         # David - Color system variables
│   └── aesthetic.scss           # David - Main entry point (renamed from main.scss)
├── .vscode/
│   └── settings.json            # VS Code Sass compiler configuration
├── dist/                        # Distribution folder (auto-generated)
│   ├── aesthetic.css            # Compiled CSS output
│   ├── aesthetic.min.css        # Minified CSS output
│   └── aesthetic.css.map        # Source map for debugging
├── examples/
│   └── demo.html                # David - Demo showcase file
├── instructions.md              # David - Team workflow guide
│
└── README.md                    # David - Project documentation
```

## Development

### Prerequisites
- Node.js and npm
- Sass compiler

### Setup
```bash
git clone <repository-url>
cd aesthetic_css_framework
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

## Examples

Check out the `examples/demo.html` file to see the Aesthetic CSS Framework in action with all styled elements and utility classes.

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
- Initial release of Aesthetic CSS Framework
- Base HTML element styling for headings, buttons, forms, tables, lists
- Utility classes for colors, typography, spacing, borders, and display
- Sass variable system for easy customization
- Responsive design principles
- Complete documentation and examples
### Key Changes in v1.0.1:
- **Renamed** `main.scss` → `aesthetic.scss` for consistent naming
- **Added** `.vscode/settings.json` for Sass compiler configuration
- **Enhanced** build system with proper CSS output naming
- **Improved** development workflow with VS Code integration