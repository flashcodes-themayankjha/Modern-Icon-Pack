# Modern Icon Pack

A sleek and versatile collection of modern SVG icons designed for various web and application projects. This icon pack provides a wide range of commonly used icons, all in a scalable vector graphics format for optimal performance and visual quality across different screen sizes.

## Installation

You can install the Modern Icon Pack via npm:

```bash
npm install modern-icon-pack
```

## Usage

### React / Vite Projects

For React and Vite projects, you can import individual icons as components.

1.  **Import the desired icon:**

    ```javascript
    import { Activity } from 'modern-icon-pack/react';
    // Or for a specific icon:
    // import { Camera } from 'modern-icon-pack/react';
    ```

2.  **Use the icon as a component in your JSX:**

    ```jsx
    function MyComponent() {
      return (
        <div>
          <Activity width="24" height="24" color="blue" />
          {/* <Camera width="32" height="32" strokeWidth="2" /> */}
        </div>
      );
    }
    ```

    *   `width` and `height`: Control the size of the icon.
    *   `color`: Sets the stroke color of the icon.
    *   `strokeWidth`: Adjusts the thickness of the icon's lines.
    *   Any other SVG attributes can also be passed as props.

### HTML Projects (Direct SVG)

For plain HTML projects, you can directly embed the SVG code or link to the SVG files.

1.  **Directly embed SVG:**
    Copy the SVG code from the desired icon file (e.g., `activity.svg`) and paste it directly into your HTML.

    ```html
    <!-- Example for activity.svg -->
    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-activity">
        <polyline points="22 12 18 12 15 21 9 3 6 12 2 12"></polyline>
    </svg>
    ```

2.  **Using `<img>` tag:**
    You can also use the SVG files directly with an `<img>` tag. Ensure the path to the SVG file is correct.

    ```html
    <img src="./path/to/icons/activity.svg" alt="Activity Icon" width="24" height="24" />
    ```

## Contributing

We welcome contributions to the Modern Icon Pack! If you have new icon ideas, improvements, or bug fixes, please feel free to open an issue or submit a pull request.

## License

This icon pack is open-source and distributed under the [MIT License](https://opensource.org/licenses/MIT).
