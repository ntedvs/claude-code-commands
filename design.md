# Design Language Creation Prompt

You are tasked with creating a comprehensive design language for a web project using Tailwind CSS.

## Research Phase

**Before creating the design system:**

- Search for existing design systems and style guides that match the project requirements
- Research current design trends and best practices for the specified aesthetic
- Look for inspiration from established design systems (Material Design, Apple HIG, etc.)
- Base your design language on proven patterns and modern standards

## User Requirements Gathering

**If the user has not specified design preferences, prompt them for:**

- Color palette preferences and brand colors
- Typography style (modern, classic, playful, corporate, etc.)
- Overall aesthetic direction (minimalist, bold, elegant, brutalist, etc.)
- Target audience and use case

## Technical Implementation Requirements

**Critical Tailwind Constraints:**

- **No self-referencing**: Cannot reference custom Tailwind classes within other custom classes (e.g., `.btn-primary` cannot use `@apply btn`)
- **No redundant styles**: Do not create custom styles for properties that Tailwind already provides utilities for (text size, shadows, etc.)
- **No comments**: Write clean CSS without comments in the design file
- Use `@apply` directive for all utility applications
- Organize code using `@theme`, `@layer base`, `@layer components`, and `@layer utilities`
- Store all styles in the main CSS file where Tailwind is imported
- Minimize redundancies and maintain DRY principles

## Implementation Strategy

1. **Theme Configuration** (`@theme`):

   - Custom color palette with semantic naming
   - Typography scale and font families
   - Spacing system and breakpoints
   - Border radius, shadows, and animation values

2. **Base Layer** (`@layer base`):

   - Reset and normalize styles
   - Typography hierarchy (h1-h6, p, etc.)
   - Form element defaults
   - Link and focus styles

3. **Components Layer** (`@layer components`):

   - Button variants (.btn-primary, .btn-secondary, etc.)
   - Form components (.input, .select, .checkbox, etc.)
   - Card and container styles
   - Navigation components

4. **Utilities Layer** (`@layer utilities`):
   - Project-specific utility classes
   - Complex spacing or layout utilities
   - Custom responsive variants

## Additional Considerations

- **Naming Conventions**: Use clear, semantic class names
- **Responsive Design**: Ensure all components work across breakpoints
- **Accessibility**: Include focus states, color contrast, and screen reader considerations

## Deliverable

Provide a complete, production-ready CSS file with:

- Clear organization using Tailwind layers
- Comprehensive component library
- Usage examples for each component
- Responsive and accessible implementations
