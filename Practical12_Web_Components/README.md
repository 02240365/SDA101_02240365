# Custom Card Component

This exercise demonstrates a reusable, customizable card component built using Web Components. The component uses Shadow DOM for style encapsulation and includes slots for different content areas.


# Project Structure

**index.html**- Main HTML file containing the structure to use the custom-card component.

**card.js** - JavaScript file defining the custom-card Web Component.


# Usage

Below is an example usage of the custom-card component. This code demonstrates how to use the component with different slots and customized styles.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Custom Card Component</title>
    <!-- Link the JavaScript file for the custom element -->
    <script src="card.js" defer></script>
    <!-- Some additional custom styles for demonstration -->
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            background-color: #000000;
        }
        custom-card {
            --card-background: #ffffff;
            --card-border-radius: 8px;
            --card-padding: 16px;
            --header-color: #ff009d;
            --footer-color: #ff009d;
        }
    </style>
</head>
<body>

    <!-- Use the custom card component -->
    <custom-card>
        <!-- Defining content for each slot -->
        <div slot="header">Card Header</div>
        <div slot="content">This is the main content area of the card. You can add text, images, or other HTML elements here.</div>
        <div slot="footer">Card Footer</div>
    </custom-card>

</body>
</html>
```
# Explanation of Code
## HTML Structure:

The <custom-card> component is used to display a card with customizable sections.

### Slots:

**Header Slot**: Displays header content with customizable colors.

**Content Slot**: The main area where text, images, or other HTML elements can be added.

**Footer Slot**: Typically used for footer information or action links.

## Customization:

Global styles are applied using CSS custom properties:

**card-background**: Sets the background color of the card.

**card-border-radius**: Controls the border radius of the card.

**card-padding**: Adjusts padding around the card content.

**header-color & footer-color**: Customizes colors for the header and footer sections.