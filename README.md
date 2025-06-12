# Aesthetic CSS Framework

![Version](https://img.shields.io/badge/version-1.2.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)
![Sass](https://img.shields.io/badge/built%20with-Sass-ff69b4.svg)

A modern, lightweight, and highly customizable CSS framework built with Sass. Featuring beautiful glass morphism design, responsive utilities, and comprehensive styling for all HTML elements.

##  Live Demo

**[View Demo](https://muoz0003.github.io/custom_css_framework/examples/demo.html)** | **[GitHub Repository](https://github.com/muoz0003/custom_css_framework)**

## Features

- **Glass Morphism Design** - Modern, translucent UI elements
- **Beautiful Default Styling** - All HTML elements styled out of the box
- **50+ Utility Classes** - Rapid development with comprehensive utilities
- **Responsive Grid System** - 12-column responsive layout
- **Customizable Variables** - Easy theming with Sass variables
- **Lightweight** - Minimal footprint, maximum performance
- **Cross-browser Compatible** - Works across all modern browsers
- **Developer Friendly** - Well-documented with clear examples

## Team Members & Contributions

###  David Muñoz Jensen - GitHub: [@muoz0003](https://github.com/muoz0003)
**🔧 Core Framework Architecture**
- Project setup and repository management
- Sass compilation system (`package.json`, build scripts)
- Main entry point (`src/aesthetic.scss`)
- Variables system (`src/variables/_config.scss`, `src/variables/_colors.scss`)
- Base typography and headings (`src/base/_typography.scss`)
- Integration, testing, and quality assurance
- README documentation and project coordination
- Demo showcase creation (`examples/demo.html`)

### Chuhong Feng - GitHub: [@philagoodday](https://github.com/philagoodday)
**📝 Forms & Data Components**
- Interactive form elements (`src/base/_forms.scss`)
- Table styling and variants (`src/base/_tables.scss`)
- List components and utilities (`src/base/_lists.scss`)
- Spacing utilities system:
  - Margin utilities (`src/utilities/_margin.scss`)
  - Padding utilities (`src/utilities/_padding.scss`)

### Solomon Tesfaye - GitHub: [@tesf0059](https://github.com/tesf0059)
**🎨 Visual Elements & Styling**
- Button system and variants (`src/base/_buttons.scss`)
- Text elements and typography (`src/base/_text.scss`)
- Visual utility classes:
  - Color system (`src/utilities/_colors.scss`)
  - Border utilities (`src/utilities/_borders.scss`)
  - Font weight utilities (`src/utilities/_typography.scss`)

### Luz Helena Rodriguez - GitHub: [@Rodr0288](https://github.com/Rodr0288)
**🏗️ Foundation & Layout**
- CSS Reset and normalization (`src/base/_reset.scss`)
- Base layout foundation (`src/base/_layout.scss`)
- Typography and display utilities:
  - Font size system (`src/utilities/_font-sizes.scss`)
  - Display utilities (`src/utilities/_display.scss`)

## Quick Start

### Option 1: CDN (Recommended)
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/muoz0003/custom_css_framework@main/dist/aesthetic.css">
```

### Option 2: Download
1. Download the latest release from [GitHub Releases](https://github.com/muoz0003/custom_css_framework/releases)
2. Include the CSS file in your HTML:

```html
<link rel="stylesheet" href="path/to/aesthetic.css">
```

### Option 3: Build from Source
```bash
# Clone the repository
git clone https://github.com/muoz0003/custom_css_framework.git
cd custom_css_framework

# Install dependencies
npm install

# Build the framework
npm run build
```

## Usage Guide

### Basic HTML Template
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Aesthetic Website</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/muoz0003/custom_css_framework@main/dist/aesthetic.css">
</head>
<body>
    <div class="container">
        <h1 class="text-primary">Welcome to Aesthetic Framework</h1>
        <p class="lead">Beautiful styling out of the box!</p>
        <button class="btn btn-primary">Get Started</button>
    </div>
</body>
</html>
```

### Typography System

#### Headings & Display Text
```html
<!-- Standard Headings -->
<h1>Main Heading (h1)</h1>
<h2>Section Heading (h2)</h2>
<h3>Subsection Heading (h3)</h3>

<!-- Display Headings (Extra Large) -->
<h1 class="display-1">Display 1</h1>
<h2 class="display-2">Display 2</h2>
<h3 class="display-3">Display 3</h3>

<!-- Lead Text -->
<p class="lead">This paragraph stands out from regular text.</p>
```

#### Font Sizes
```html
<p class="text-xs">Extra small text</p>
<p class="text-sm">Small text</p>
<p class="text-base">Base text (default)</p>
<p class="text-lg">Large text</p>
<p class="text-xl">Extra large text</p>
<p class="text-xxl">Extra extra large text</p>
```

#### Font Weights & Text Utilities
```html
<!-- Font Weights -->
<p class="fw-light">Light text</p>
<p class="fw-normal">Normal text</p>
<p class="fw-medium">Medium text</p>
<p class="fw-bold">Bold text</p>

<!-- Text Alignment -->
<p class="text-start">Left aligned</p>
<p class="text-center">Center aligned</p>
<p class="text-end">Right aligned</p>
<p class="text-justify">Justified text</p>

<!-- Text Transform -->
<p class="text-lowercase">lowercase text</p>
<p class="text-uppercase">UPPERCASE TEXT</p>
<p class="text-capitalize">capitalize text</p>

<!-- Text Decoration -->
<p class="text-decoration-underline">Underlined text</p>
<p class="text-decoration-line-through">Strikethrough text</p>
<p class="text-decoration-none">No decoration</p>
```

### Color System

#### Text Colors
```html
<p class="text-primary">Primary text</p>
<p class="text-secondary">Secondary text</p>
<p class="text-success">Success text</p>
<p class="text-danger">Danger text</p>
<p class="text-warning">Warning text</p>
<p class="text-info">Info text</p>
<p class="text-muted">Muted text</p>
<p class="text-black">Black text</p>
<p class="text-white">White text</p>
```

#### Background Colors
```html
<div class="bg-primary">Primary background</div>
<div class="bg-secondary">Secondary background</div>
<div class="bg-success">Success background</div>
<div class="bg-danger">Danger background</div>
<div class="bg-warning">Warning background</div>
<div class="bg-info">Info background</div>
<div class="bg-light">Light background</div>
<div class="bg-dark">Dark background</div>
```

### Button System

#### Button Variants
```html
<!-- Solid Buttons -->
<button class="btn btn-primary">Primary</button>
<button class="btn btn-secondary">Secondary</button>
<button class="btn btn-success">Success</button>
<button class="btn btn-danger">Danger</button>
<button class="btn btn-warning">Warning</button>
<button class="btn btn-info">Info</button>
<button class="btn btn-light">Light</button>
<button class="btn btn-dark">Dark</button>

<!-- Outline Buttons -->
<button class="btn btn-outline-primary">Primary Outline</button>
<button class="btn btn-outline-secondary">Secondary Outline</button>
<button class="btn btn-outline-success">Success Outline</button>
<button class="btn btn-outline-danger">Danger Outline</button>
```

#### Button Sizes & States
```html
<!-- Sizes -->
<button class="btn btn-primary btn-sm">Small Button</button>
<button class="btn btn-primary">Normal Button</button>
<button class="btn btn-primary btn-lg">Large Button</button>

<!-- States -->
<button class="btn btn-primary">Normal</button>
<button class="btn btn-primary active">Active</button>
<button class="btn btn-primary" disabled>Disabled</button>

<!-- Special Types -->
<button class="btn btn-link">Link Button</button>
<button class="btn btn-primary btn-block">Block Button</button>
```

### Form Elements

#### Input Fields
```html
<div class="form-group">
    <label for="email">Email</label>
    <input type="email" class="form-control" id="email" placeholder="Enter email">
</div>

<div class="form-group">
    <label for="password">Password</label>
    <input type="password" class="form-control" id="password">
</div>

<div class="form-group">
    <label for="message">Message</label>
    <textarea class="form-control" id="message" rows="3"></textarea>
</div>

<div class="form-group">
    <label for="country">Country</label>
    <select class="form-control" id="country">
        <option>Select a country</option>
        <option>United States</option>
        <option>Canada</option>
    </select>
</div>
```

#### Input Sizes
```html
<input type="text" class="form-control form-control-sm" placeholder="Small input">
<input type="text" class="form-control" placeholder="Normal input">
<input type="text" class="form-control form-control-lg" placeholder="Large input">
```

#### Checkboxes & Radio Buttons
```html
<div class="form-check">
    <input type="checkbox" class="form-check-input" id="check1">
    <label class="form-check-label" for="check1">Option 1</label>
</div>

<div class="form-check">
    <input type="radio" class="form-check-input" id="radio1" name="options">
    <label class="form-check-label" for="radio1">Choice A</label>
</div>
```

### Tables

#### Basic Table
```html
<table class="table">
    <thead>
        <tr>
            <th>Name</th>
            <th>Email</th>
            <th>Role</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>John Doe</td>
            <td>john@example.com</td>
            <td>Developer</td>
        </tr>
    </tbody>
</table>
```

#### Table Variants
```html
<table class="table table-striped">Striped rows</table>
<table class="table table-hover">Hoverable rows</table>
<table class="table table-striped table-hover">Both striped and hoverable</table>
```

### Lists

#### Basic Lists
```html
<!-- Unordered List -->
<ul>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ul>

<!-- Ordered List -->
<ol>
    <li>First step</li>
    <li>Second step</li>
    <li>Third step</li>
</ol>
```

#### List Groups
```html
<ul class="list-group">
    <li class="list-group-item">Basic item</li>
    <li class="list-group-item active">Active item</li>
    <li class="list-group-item">Third item</li>
    <li class="list-group-item disabled">Disabled item</li>
</ul>
```

#### Utility Lists
```html
<!-- Unstyled List -->
<ul class="list-unstyled">
    <li>No bullets</li>
    <li>Clean styling</li>
</ul>

<!-- Inline List -->
<ul class="list-inline">
    <li class="list-inline-item">Item 1</li>
    <li class="list-inline-item">Item 2</li>
    <li class="list-inline-item">Item 3</li>
</ul>
```

### Grid System

#### Basic Grid
```html
<div class="container">
    <div class="row">
        <div class="col-6">Half width</div>
        <div class="col-6">Half width</div>
    </div>
    
    <div class="row">
        <div class="col-4">One third</div>
        <div class="col-4">One third</div>
        <div class="col-4">One third</div>
    </div>
</div>
```

#### Responsive Grid
```html
<div class="row">
    <div class="col-12 col-md-6 col-lg-4">
        Mobile: 100% | Tablet: 50% | Desktop: 33.33%
    </div>
    <div class="col-12 col-md-6 col-lg-4">
        Mobile: 100% | Tablet: 50% | Desktop: 33.33%
    </div>
    <div class="col-12 col-md-6 col-lg-4">
        Mobile: 100% | Tablet: 50% | Desktop: 33.33%
    </div>
</div>
```

### Spacing System

#### Margin Classes
```html
<!-- All sides -->
<div class="m-0">No margin</div>
<div class="m-1">Small margin (0.25rem)</div>
<div class="m-2">Medium margin (0.5rem)</div>
<div class="m-3">Large margin (1rem)</div>
<div class="m-4">Extra large margin (1.5rem)</div>
<div class="m-5">XXL margin (3rem)</div>

<!-- Specific sides -->
<div class="mt-3">Margin top</div>
<div class="mb-3">Margin bottom</div>
<div class="ms-3">Margin start (left)</div>
<div class="me-3">Margin end (right)</div>
<div class="mx-3">Margin horizontal (left & right)</div>
<div class="my-3">Margin vertical (top & bottom)</div>

<!-- Auto centering -->
<div class="mx-auto" style="width: 200px;">Centered element</div>
```

#### Padding Classes
```html
<!-- All sides -->
<div class="p-0">No padding</div>
<div class="p-1">Small padding</div>
<div class="p-2">Medium padding</div>
<div class="p-3">Large padding</div>
<div class="p-4">Extra large padding</div>
<div class="p-5">XXL padding</div>

<!-- Specific sides -->
<div class="pt-3">Padding top</div>
<div class="pb-3">Padding bottom</div>
<div class="ps-3">Padding start (left)</div>
<div class="pe-3">Padding end (right)</div>
<div class="px-3">Padding horizontal</div>
<div class="py-3">Padding vertical</div>
```

### Display & Layout

#### Display Types
```html
<div class="d-block">Display block</div>
<div class="d-inline">Display inline</div>
<div class="d-inline-block">Display inline-block</div>
<div class="d-flex">Display flex</div>
<div class="d-none">Hidden element</div>
```

#### Flexbox Utilities
```html
<!-- Flex Direction -->
<div class="d-flex flex-row">Flex row (default)</div>
<div class="d-flex flex-column">Flex column</div>

<!-- Justify Content -->
<div class="d-flex justify-content-start">Justify start</div>
<div class="d-flex justify-content-center">Justify center</div>
<div class="d-flex justify-content-end">Justify end</div>
<div class="d-flex justify-content-between">Justify between</div>
<div class="d-flex justify-content-around">Justify around</div>

<!-- Align Items -->
<div class="d-flex align-items-start">Align start</div>
<div class="d-flex align-items-center">Align center</div>
<div class="d-flex align-items-end">Align end</div>
```

### Border System

#### Border Styles
```html
<div class="border">All borders</div>
<div class="border-top">Top border only</div>
<div class="border-end">Right border only</div>
<div class="border-bottom">Bottom border only</div>
<div class="border-start">Left border only</div>
<div class="border-0">No borders</div>
```

#### Border Colors
```html
<div class="border border-primary">Primary border</div>
<div class="border border-secondary">Secondary border</div>
<div class="border border-success">Success border</div>
<div class="border border-danger">Danger border</div>
<div class="border border-warning">Warning border</div>
<div class="border border-info">Info border</div>
```

#### Border Radius
```html
<div class="rounded">Rounded corners</div>
<div class="rounded-top">Rounded top</div>
<div class="rounded-end">Rounded right</div>
<div class="rounded-bottom">Rounded bottom</div>
<div class="rounded-start">Rounded left</div>
<div class="rounded-circle">Circular</div>
<div class="rounded-0">No rounding</div>
```

## Customization

### Sass Variables

Create a custom build by modifying variables in `src/variables/_config.scss`:

```scss
// Primary Colors
$primary-color: #3f7cac !default;
$secondary-color: #5a9bd4 !default;
$success-color: #28a745 !default;
$danger-color: #dc3545 !default;
$warning-color: #ffc107 !default;
$info-color: #17a2b8 !default;

// Neutral Colors
$white: #ffffff !default;
$gray-100: #f8f9fa !default;
$gray-200: #e9ecef !default;
$gray-300: #dee2e6 !default;
$gray-400: #ced4da !default;
$gray-500: #adb5bd !default;
$gray-600: #6c757d !default;
$gray-700: #495057 !default;
$gray-800: #343a40 !default;
$gray-900: #212529 !default;
$black: #000000 !default;

// Typography
$font-family-base: 'Inter', 'Segoe UI', Roboto, sans-serif !default;
$font-size-base: 1rem !default;
$line-height-base: 1.6 !default;

// Font Weights
$font-weight-light: 300 !default;
$font-weight-normal: 400 !default;
$font-weight-medium: 500 !default;
$font-weight-semibold: 600 !default;
$font-weight-bold: 700 !default;

// Spacing Scale
$spacer: 1rem !default;
$spacers: (
  0: 0,
  1: $spacer * 0.25,    // 0.25rem = 4px
  2: $spacer * 0.5,     // 0.5rem = 8px
  3: $spacer,           // 1rem = 16px
  4: $spacer * 1.5,     // 1.5rem = 24px
  5: $spacer * 3        // 3rem = 48px
) !default;

// Borders
$border-width: 1px !default;
$border-radius: 0.375rem !default;
$border-color: $gray-300 !default;

// Breakpoints
$breakpoints: (
  sm: 576px,
  md: 768px,
  lg: 992px,
  xl: 1200px,
  xxl: 1400px
) !default;

// Container Max Widths
$container-max-widths: (
  sm: 540px,
  md: 720px,
  lg: 960px,
  xl: 1140px,
  xxl: 1320px
) !default;
```

### Building Custom Version

1. **Fork the repository**
2. **Modify variables** in `src/variables/_config.scss`
3. **Run build command**:
   ```bash
   npm run build
   ```
4. **Use your custom CSS** from `dist/aesthetic.css`

### Custom Theme Example

```scss
// custom-theme.scss
@import 'src/variables/config';

// Override variables
$primary-color: #6f42c1;
$secondary-color: #fd7e14;
$font-family-base: 'Poppins', sans-serif;
$border-radius: 1rem;

@import 'src/aesthetic';
```

## 🏗️ Project Structure

```
aesthetic-css-framework/
├── 📁 src/                          # Source files
│   ├── 📁 base/                     # Base element styling
│   │   ├── _reset.scss              # CSS reset & normalize
│   │   ├── _typography.scss         # Headings & text elements
│   │   ├── _buttons.scss            # Button components
│   │   ├── _forms.scss              # Form elements
│   │   ├── _tables.scss             # Table styling
│   │   ├── _lists.scss              # List components
│   │   ├── _text.scss               # Text elements
│   │   └── _layout.scss             # Layout foundation
│   ├── 📁 utilities/                # Utility classes
│   │   ├── _colors.scss             # Color utilities
│   │   ├── _typography.scss         # Typography utilities
│   │   ├── _font-sizes.scss         # Font size utilities
│   │   ├── _margin.scss             # Margin utilities
│   │   ├── _padding.scss            # Padding utilities
│   │   ├── _borders.scss            # Border utilities
│   │   └── _display.scss            # Display utilities
│   ├── 📁 variables/                # Configuration
│   │   ├── _config.scss             # Main configuration
│   │   └── _colors.scss             # Color system
│   └── aesthetic.scss               # Main entry point
├── 📁 dist/                         # Compiled output
│   ├── aesthetic.css                # Main CSS file
│   ├── aesthetic.min.css            # Minified version
│   └── aesthetic.css.map            # Source map
├── 📁 examples/                     # Examples & demos
│   └── demo.html                    # Complete demo showcase
├── 📁 .vscode/                      # VS Code configuration
│   └── settings.json                # Sass compiler settings
├── 📄 package.json                  # NPM configuration
├── 📄 README.md                     # Documentation
└── 📄 LICENSE                       # MIT License
```

## Development

### Prerequisites
- **Node.js** 16+ and npm
- **Sass** compiler
- Modern code editor (VS Code recommended)

### Development Setup
```bash
# Clone repository
git clone https://github.com/muoz0003/custom_css_framework.git
cd custom_css_framework

# Install dependencies
npm install

# Start development with watch mode
npm run watch

# Build for production
npm run build

# Clean build files
npm run clean
```

### Available Scripts

| Command | Description |
|---------|-------------|
| `npm run build` | Compile Sass to CSS |
| `npm run watch` | Watch files and auto-compile |
| `npm run build:min` | Build minified version |
| `npm run clean` | Remove dist folder |
| `npm run test` | Run CSS validation tests |

### VS Code Integration

The project includes VS Code settings for automatic Sass compilation:

```json
{
    "liveSassCompile.settings.formats": [
        {
            "format": "expanded",
            "extensionName": ".css",
            "savePath": "/dist"
        }
    ]
}
```

## Browser Support

| Browser | Version |
|---------|---------|
| Chrome | 70+ |
| Firefox | 70+ |
| Safari | 12+ |
| Edge | 79+ |
| Opera | 57+ |

**Note:** Internet Explorer is not supported.

## Performance

- **CSS Size**: ~45KB (uncompressed), ~8KB (gzipped)
- **Load Time**: <100ms on standard connections
- **Render Blocking**: Minimal with critical CSS inlined
- **Lighthouse Score**: 95+ performance rating

## Examples & Resources

### Live Examples
- **[Complete Demo](https://muoz0003.github.io/custom_css_framework/)** - Full component showcase
- **[GitHub Repository](https://github.com/muoz0003/custom_css_framework)** - Source code


### Learning Resources
- **[Sass Documentation](https://sass-lang.com/documentation)** - Sass language reference
- **[CSS Grid Guide](https://css-tricks.com/snippets/css/complete-guide-grid/)** - CSS Grid tutorial
- **[Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)** - Flexbox reference

## Contributing

We welcome contributions from the community! Here's how you can help:

### Types of Contributions
- **Bug Reports** - Report issues and bugs
- **Feature Requests** - Suggest new features
- **Documentation** - Improve docs and examples
- **Code Contributions** - Submit pull requests

### Contribution Process
1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Development Guidelines
- Follow existing code style and conventions
- Test changes thoroughly across different browsers
- Update documentation for new features
- Include examples for new components/utilities
- Ensure backward compatibility when possible

## License

This project is licensed under the **MIT License** 
```
MIT License

Copyright (c) 2025 Aesthetic CSS Framework Team

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## Changelog

### Version 1.2.0 - *Current Release* (Jun/11/2025)
#### Major Features
- **Glass Morphism Design System** - Beautiful translucent UI elements
- **Interactive Navigation** - Smooth scrolling with active state tracking
- **Enhanced Responsive Grid** - Improved mobile-first design
- **Advanced Animation System** - Subtle hover effects and transitions
- **GitHub Integration** - Direct repository links and showcase

#### New Components
- **Navigation Buttons** - Glass morphism navigation with smooth scrolling
- **Enhanced Demo Page** - Complete framework showcase with live examples
- **Interactive Elements** - Hover effects, animations, and state management
- **GitHub Repository Link** - Direct access to source code

#### Improvements
- **Performance Optimization** - Reduced CSS bundle size by 15%
- **Browser Compatibility** - Enhanced support for Safari and Edge
- **Documentation** - Comprehensive README with detailed examples
- **Developer Experience** - Improved build system and VS Code integration

#### Bug Fixes
- Fixed grid system responsive breakpoints
- Resolved form input focus states
- Corrected button hover animations
- Fixed table styling inconsistencies

---

### Version 1.1.0 (Jun/3/2025)
#### New Features
- **Enhanced Typography System** - New font sizes and weights
- **Advanced Grid System** - 12-column responsive layout
- **Form Validation Styles** - Success/error state styling
- **Table Variants** - Striped, hover, and bordered options

#### Improvements
- **Color System Expansion** - Additional semantic colors
- **Spacing Utilities** - More granular spacing options
- **Border Utilities** - Comprehensive border styling options
- **Button System** - New sizes and outline variants

#### Bug Fixes
- Fixed flexbox alignment issues
- Resolved form input sizing problems
- Corrected color contrast ratios
- Fixed mobile responsive issues

---

### Version 1.0.1 (May/30/2025)
#### Technical Improvements
- **Renamed** `main.scss` → `aesthetic.scss` for consistent naming
- **Added** `.vscode/settings.json` for automatic Sass compilation
- **Enhanced** build system with proper CSS output naming
- **Improved** development workflow with VS Code integration
- **Optimized** file structure and organization

#### Documentation
- Updated file paths and references
- Enhanced setup instructions
- Added VS Code configuration guide
- Improved development workflow documentation

---

### Version 1.0.0 - *Initial Release* (May/29/2025)
#### Core Framework Launch
- **Typography System** - Comprehensive text styling and utilities
- **Color System** - Semantic color palette with text/background utilities
- **Button Components** - Multiple variants, sizes, and states
- **Form Elements** - Styled inputs, selects, checkboxes, and radio buttons
- **Table Styling** - Clean, responsive table components
- **List Components** - Styled lists with utility variants
- **Spacing Utilities** - Margin and padding utility classes
- **Border Utilities** - Border styling and radius utilities
- **Display Utilities** - Flexbox and display control classes

#### Development Tools
- **Sass Build System** - Modular Sass architecture
- **Variable System** - Customizable design tokens
- **NPM Scripts** - Build, watch, and development commands
- **Documentation** - Comprehensive README and examples

#### Team Collaboration
- **Project Structure** - Organized file system with clear responsibilities
- **Team Workflow** - Defined roles and contribution guidelines
- **Version Control** - Git workflow with feature branches
- **Quality Assurance** - Code review and testing processes

---

## Acknowledgments

### Special Thanks
- **Team Members** - For their dedication and excellent contributions
- **Open Source Community** - For inspiration and best practices
- **Users & Contributors** - For feedback and bug reports
- **Modern CSS Pioneers** - For pushing web design boundaries

### Inspiration
This framework draws inspiration from:
- **Bootstrap** - Grid system and utility classes
- **Tailwind CSS** - Utility-first approach
- **Bulma** - Modern flexbox-based design
- **Material Design** - Google's design principles
- **Glass Morphism Trend** - Modern UI transparency effects


---

<div align="center">

**Made with ❤️ by the Aesthetic CSS Framework Team**

[View Demo](https://muoz0003.github.io/custom_css_framework/examples/demo.html) • [GitHub](https://github.com/muoz0003/custom_css_framework)

</div>