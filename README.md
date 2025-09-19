# This project has been developed by Abdul Aliyan
﻿# VIZUME - PORTFOLIO  WEBSITE


# Overview

Vizume is a portfolio builder web application that allows users to create professional portfolios through an interactive form interface. The application consists of two main components: a portfolio builder interface where users input their personal information and project details, and a preview system that dynamically renders a professional-looking portfolio website. Users can customize themes, add multiple projects, and download their completed portfolio as a standalone website package.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
The application uses a vanilla JavaScript class-based architecture with separate concerns for building and previewing portfolios. The `PortfolioBuilder` class handles form interactions, data collection, and project management, while the `PortfolioPreview` class manages portfolio rendering and theme switching. The interface leverages Bootstrap 5 for responsive design and Font Awesome for iconography.

## Data Storage Strategy
Portfolio data is stored client-side using localStorage, eliminating the need for backend infrastructure. This approach provides immediate data persistence across sessions while keeping the application lightweight and deployable on static hosting platforms. The data structure includes personal information (name, email, phone, profession, experience) and project arrays with associated metadata.

## Theme System
A CSS custom properties-based theming system supports light and dark modes with smooth transitions. Theme preferences are persisted in localStorage and applied dynamically through data attributes on the document root, allowing for real-time theme switching without page reloads.

## Project Management
Dynamic project addition/removal functionality with configurable limits (minimum 2, maximum 6 projects). Each project includes fields for title, description, technologies used, and project links. The system includes smooth animations for adding and removing project sections to enhance user experience.

## Asset Handling
Profile images are processed client-side using the File API and converted to base64 format for storage and display. This eliminates the need for file upload servers while maintaining image persistence across sessions.

## Responsive Design
Mobile-first responsive design using CSS Grid and Flexbox layouts with Bootstrap components. The navigation includes a hamburger menu for mobile devices and smooth scrolling between portfolio sections.

# External Dependencies

## UI Frameworks
- **Bootstrap 5.3.7**: Provides responsive grid system, form components, and utility classes for rapid UI development
- **Font Awesome 6.4.0**: Icon library for UI elements including social media icons, navigation indicators, and action buttons

## Fonts
- **Google Fonts (Inter)**: Modern sans-serif font family with multiple weights (300-800) for typography consistency and professional appearance

## Animation Libraries
- **AOS (Animate On Scroll) 2.3.1**: Provides smooth scroll-triggered animations for portfolio sections in the preview interface

## Browser APIs
- **File API**: For client-side image processing and base64 conversion
- **localStorage API**: For persistent data storage without requiring a backend database
- **CSS Custom Properties**: For dynamic theming system implementation

The application is designed to be fully self-contained with no server-side dependencies, making it suitable for static hosting environments like GitHub Pages, Netlify, or similar platforms.# vizume
# vizume


