# Module 02: Antora

### Brief Overview

This module explains the Antora documentation site structure and configuration. Participants learn how the antora.yml component descriptor defines the site structure, how nav.adoc controls navigation, and how modules organize content into logical units. The module covers the YAML keys used in ui-config.yml and site.yml, including how the modules list with name and label properties generates navigation menus automatically.

### Audience and Time

- **Target personas:** Lab authors, documentation architects, site maintainers
- **Prerequisites for this module:** Familiarity with YAML syntax and basic understanding of web documentation structure
- **Estimated duration:** 10 minutes

### Learning Objectives

- Recognize the antora configuration section in ui-config.yml
- Understand basic Antora directory and module structure
- Identify how name and label properties are used in module configuration

### Lab Structure

| Section | Title | Duration |
|---------|-------|----------|
| 1       | The Antora Component Descriptor | 3 min |
| 2       | Configuration Keys and Navigation | 4 min |
| 3       | Module Hierarchy and Content Organization | 3 min |

### Detailed Steps

1. Locate the antora.yml file in your content directory and examine its structure
2. Identify the key fields: name (component name), version, title, and nav (navigation file)
3. Open nav.adoc and observe how it defines the content hierarchy with page references
4. Understand that each line in nav.adoc (with indentation) represents a navigation entry and file path
5. Check ui-config.yml to see how the modules list is structured with name and label properties
6. Understand that the name property corresponds to the directory in content/modules/ (e.g., ROOT for content/modules/ROOT/)
7. Observe that the label property is the display name shown in the navigation menu
8. Verify that modifying the label in ui-config.yml automatically updates the navigation menu title without changing the actual directory structure

### Key Takeaways

- Antora uses a hierarchical structure: component > modules > pages
- antora.yml defines the component metadata and points to nav.adoc for navigation structure
- nav.adoc is an AsciiDoc file that defines the navigation tree and page references
- ui-config.yml modules list maps directory names to display labels for the navigation UI
- Proper YAML indentation and file references are critical for correct navigation generation
- Changes to configuration are reflected automatically when the site is rebuilt

### Infrastructure Notes

None — this module covers configuration and markup structure only.
