🧩 Click and Reveal: Four Quadrants

A premium, dashboard-inspired interactive layout designed for categorized learning. This component presents four distinct topics in a balanced grid, allowing users to dive deep into specific content via an immersive modal system.

🚀 Live Demo

Explore the Four Quadrants Interactive Here

✨ Project Overview

The "Four Quadrants" component is optimized for comparison tasks, SWOT analyses, or any educational content divided into four logical categories. It prioritizes a clean, high-end aesthetic that fits seamlessly into corporate and academic training modules.

Key Features

Responsive Dashboard Grid: Uses CSS Grid to transition from a 2x2 layout on desktops to a focused single-column list on mobile devices.

Immersive Modals: Deep-dive content is presented in high-contrast modals with backdrop blurring (backdrop-filter) for maximum focus.

Visual Continuity: Integrated SVG iconography and consistent brand colors (Midnight Blue and Teal) reinforce professional wayfinding.

Accentuated Details: Each modal features a "Focus Point" box, perfect for key takeaways, definitions, or "pro-tips."

🛠️ Technical Implementation

Stateful Modals: Uses a lightweight JavaScript transition engine that handles the display: none to display: flex switch alongside CSS opacity and scale transforms for a smooth "pop-in" effect.

Outside-In Interaction: Includes an "Outside Click" listener (closeModalOnOutsideClick), allowing users to dismiss modals by clicking the darkened backdrop, improving UX.

Reflow Management: Employs modal.offsetHeight triggering to ensure CSS transitions execute correctly when elements are changed from hidden to visible states.

Tailwind Integrated: Leverages Tailwind CSS for typography and layout utility, while custom CSS handles complex animations and brand-specific borders.

📂 Design Tokens

Midnight Blue (#1f2a52): Primary theme color for headers and buttons.

Teal (#00bec7): Accent color for icons, hover states, and modal highlight borders.

Light Aqua (#d2f0f0): Soft background for icons and secondary borders.

Inter Font: High-legibility sans-serif typeface optimized for UI text.

📖 Usage Instructions

Customizing Content

To update the text for a quadrant, modify the dashboard-card div in the HTML. For the deep-dive content, locate the corresponding modal div.

Modifying the Layout

The grid is controlled by these classes in the <style> block:

/* Desktop: 2 columns */
@media (min-width: 768px) {
    .quadrant-grid {
        grid-template-columns: repeat(2, 1fr);
    }
}

/* Mobile: Default to 1 column */
.quadrant-grid {
    grid-template-columns: repeat(1, 1fr);
}


📄 License

MIT License - Part of the accounts-eles UI component library.
