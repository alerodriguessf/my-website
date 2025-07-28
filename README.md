

# **Minimalist Personal Portfolio Website**

## **Project Overview**

This repository contains the source code for my personal portfolio website, designed and hand-coded from the ground up using the [Astro](https://astro.build/) framework. The primary objective of this project was to create a lightweight, content-focused, and high-performance showcase for my data and engineering projects.

The design philosophy is deliberately minimalist, prioritizing fast load times and a clean, unobtrusive user experience. By avoiding heavy JavaScript frameworks and complex CSS libraries, the site ensures that the focus remains squarely on the content.

## **Table of Contents**

1.  Architectural Design & Key Features
2.  Tech Stack
3.  Project Structure
4.  Local Development & Setup
5.  Conclusion & Future Work

-----

## **Architectural Design & Key Features**

This website is built as a static, single-page application, leveraging Astro's component-based architecture for modularity and reusability.

  * **Static-First Approach**: The site is rendered to static HTML at build time, resulting in exceptional performance and SEO-friendliness.
  * **Component-Based Architecture**: The UI is broken down into logical, reusable components (`Navbar`, `Portfolio`, `AboutMe`, etc.), making the codebase clean and maintainable. Each component encapsulates its own structure and styling.
  * **Minimalist Styling**: Styling is primarily handled via scoped CSS within Astro components and a lean global stylesheet. This choice avoids the overhead of larger CSS frameworks and demonstrates proficiency with core web technologies.
  * **Content as Data**: Project information is managed within a JavaScript array inside the `Portfolio.astro` component, serving as a simple, self-contained data source.
  * **Interactive Elements**: Subtle interactivity, such as hover effects and a "copy to clipboard" button, is implemented with minimal vanilla JavaScript to enhance user experience without compromising performance.

-----

## **Tech Stack**

  * **Framework**: [Astro](https://astro.build/) (v5.10.1)
  * **Styling**: CSS & Inline Styles
  * **Deployment**: This project is configured for easy deployment on platforms like Netlify, Vercel, or GitHub Pages.

-----

## **Project Structure**

The codebase is organized logically to separate concerns and facilitate maintainability.

```
/
├── public/              # Static assets (images, favicon)
├── src/
│   ├── components/      # Reusable Astro components (Navbar, Portfolio, etc.)
│   ├── layouts/         # Base layout for all pages
│   └── pages/           # Main page of the website (index.astro)
├── astro.config.mjs     # Astro configuration file
└── package.json         # Project dependencies and scripts
```

-----

## **Local Development & Setup**

To run this project in a local development environment, follow these steps:

1.  **Clone the repository**:

    ```bash
    git clone https://github.com/alerodriguessf/my_website.git
    cd my_website
    ```

2.  **Install dependencies**:
    This project uses `npm`. Ensure you have Node.js installed.

    ```bash
    npm install
    ```

3.  **Run the development server**:
    This command starts a local server, typically at `http://localhost:4321`.

    ```bash
    npm run dev
    ```

-----

## **Conclusion & Future Work**

This project successfully meets the goal of creating a fast, minimalist, and professional portfolio. It effectively demonstrates skills in modern web development practices and a keen eye for design and performance.

Potential future enhancements include:

  * **Refactor Styling**: Migrate inline styles to a more scalable solution like CSS Modules or a utility-first framework like Tailwind CSS to improve maintainability.
  * **Headless CMS Integration**: Abstract the project data from the component into a headless CMS (e.g., Contentful, Sanity) to allow for easier content updates without code changes.
  * **Accessibility (A11y) Audit**: Perform a thorough accessibility audit to ensure the site is usable for all visitors, including those using assistive technologies.
  * **Add View Transitions**: Implement Astro's native View Transitions API to create seamless, animated page transitions if the site expands to multiple pages.
