# Reflection on Web Components



## Main Concepts Applied

-**Web Components**: The project uses the concept of custom HTML elements, specifically creating a <custom-card> element. Web Components allow you to define reusable elements that encapsulate their structure, style, and behavior.

-**Shadow DOM**: Inside the JavaScript file (card.js), the component likely uses the Shadow DOM to keep its styles and structure isolated from the rest of the document. This ensures that the component’s design remains unaffected by external CSS.

-**Slot Mechanism**: Slots are used to define specific areas (header, content, footer) within the card, allowing for flexible insertion of different types of content. This makes the component reusable with custom content.






## New Skills or Knowledge Gained


-**Custom HTML Elements**: Creating and implementing custom HTML elements with JavaScript.

-**CSS Custom Properties**: The card’s design utilizes CSS custom properties (e.g., --card-background, --header-color). This enables easy customization without modifying the core component.

-**Encapsulation of Styles**: Through the use of Shadow DOM, the component’s styles are encapsulated, which helps in avoiding conflicts with global CSS styles.





## Challenges Faced and Overcoming Them


-**Challenge**: Getting the slots to display the content correctly within the card component was initially difficult. The content didn’t render until I properly specified the slot attribute in the HTML.

**Solution**: I consulted the documentation on using slots within web components, which clarified that I needed to define slot="header", slot="content", and slot="footer" attributes for each respective area.

-**Challenge**: Centering the <custom-card> on the page was tricky since the body CSS was not applying to the Shadow DOM.

**Solution**: I added custom styles directly within the component’s Shadow DOM and used flexbox properties in the body’s CSS to center the component horizontally and vertically.

