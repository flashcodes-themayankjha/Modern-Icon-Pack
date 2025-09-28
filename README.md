# Modern Icon Pack

A sleek and versatile collection of modern SVG icons designed for various web and application projects. This icon pack provides a wide range of commonly used icons, all in a scalable vector graphics format for optimal performance and visual quality across different screen sizes.

## Installation

You can install the Modern Icon Pack via npm:

```bash
npm install @mayankjha07/modern-icons
```

## Usage

This package is designed to be used with a build process that converts the raw SVG files into components (e.g., React components). The examples below assume such a build process is in place.

### Main Icons (React / Vite Projects)

Main icons are organized by style (Outline, Filled, Colored). The existing icons are in the `Outline` style.

1.  **Import the desired icon:**

    ```javascript
    // For an outline icon (e.g., Activity)
    import { Activity } from '@mayankjha07/modern-icons/icons/Outline';

    // If Filled or Colored versions were available:
    // import { Camera } from '@mayankjha07/modern-icons/icons/Filled';
    ```

2.  **Use the icon as a component in your JSX:**

    ```jsx
    function MyComponent() {
      return (
        <div>
          <Activity width="24" height="24" color="blue" />
        </div>
      );
    }
    ```

    *   `width` and `height`: Control the size of the icon.
    *   `color`: Sets the stroke color of the icon.
    *   `strokeWidth`: Adjusts the thickness of the icon's lines.
    *   Any other SVG attributes can also be passed as props.

### Social Icons (React / Vite Projects)

Social icons are organized by style (Colored, Filled, Outline) and then by type (Normal, Badge, Round, Square).

1.  **Import the desired social icon:**

    ```javascript
    // For a normal colored Facebook icon
    import { Facebook } from '@mayankjha07/modern-icons/social/Colored/Normal';

    // For a round filled Facebook icon
    // import { FacebookRoundFilled } from '@mayankjha07/modern-icons/social/Filled/Round';
    ```

2.  **Use the icon as a component in your JSX:**

    ```jsx
    function SocialComponent() {
      return (
        <div>
          <Facebook size="24" color="#1877F2" />
        </div>
      );
    }
    ```

### System Design Icons (React / Vite Projects)

System design icons are organized by style (Coloured, Filled, Outline) and then by type (Normal, Badge, Round, Square).

1.  **Import the desired system design icon:**

    ```javascript
    // For a normal coloured CloudConnection icon
    import { CloudConnection } from '@mayankjha07/modern-icons/system-designs/Coloured/Normal';

    // For a badge coloured AddCloud icon
    // import { AddCloudBadge } from '@mayankjha07/modern-icons/system-designs/Coloured/Badge';
    ```

2.  **Use the icon as a component in your JSX:**

    ```jsx
    function SystemDesignComponent() {
      return (
        <div>
          <CloudConnection size="24" color="purple" />
        </div>
      );
    }
    ```

### Dynamic Component Usage (Requires Build Process)

To achieve dynamic usage like `<Instagram style="round" type="badge" />`, you would need a build process that generates a single component capable of resolving the correct SVG based on the `style` and `type` props. This package provides the organized SVG assets, and a build tool would be responsible for creating such dynamic components.

### HTML Projects (Direct SVG)

For plain HTML projects, you can directly embed the SVG code or link to the SVG files. You can access the raw SVG files directly from the `icons`, `Social-icons`, and `System-Designs-Icon` directories within the installed `node_modules/@mayankjha07/modern-icons` package, following the new folder structure.

1.  **Directly embed SVG:**
    Copy the SVG code from the desired icon file (e.g., `node_modules/@mayankjha07/modern-icons/icons/Outline/activity.svg`) and paste it directly into your HTML.

    ```html
    <!-- Example for activity.svg -->
    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-activity">
        <polyline points="22 12 18 12 15 21 9 3 6 12 2 12"></polyline>
    </svg>
    ```

2.  **Using `<img>` tag:**
    You can also use the SVG files directly with an `<img>` tag. Ensure the path to the SVG file is correct relative to your project structure or build process.

    ```html
    <img src="./node_modules/@mayankjha07/modern-icons/icons/Outline/activity.svg" alt="Activity Icon" width="24" height="24" />
    ```

## Contributing

We welcome contributions to the Modern Icon Pack! If you have new icon ideas, improvements, or bug fixes, please feel free to open an issue or submit a pull request.

## License

This icon pack is open-source and distributed under the [MIT License](https://opensource.org/licenses/MIT).
