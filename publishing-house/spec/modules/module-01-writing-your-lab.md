# Module 01: Writing your lab

### Brief Overview

This module introduces AsciiDoc syntax and variable usage in the Showroom lab framework. Participants learn how to reference variables defined in site.yml (such as lab_name) and insert images using Antora's image macro syntax. The module covers AsciiDoc fundamentals, variable interpolation in markup, and the proper macro format for embedding images in lab documentation.

### Audience and Time

- **Target personas:** Lab authors, technical writers, content developers
- **Prerequisites for this module:** Basic familiarity with YAML files and text editors
- **Estimated duration:** 10 minutes

### Learning Objectives

- Configure AsciiDoc variables defined in site.yml and reference them in lab content using the variable interpolation syntax
- Insert images using Antora's image macro with proper path references and optional parameters
- Understand the basic structure of AsciiDoc files and how variables enhance content reusability

### Lab Structure

| Section | Title | Duration |
|---------|-------|----------|
| 1       | AsciiDoc Variables and site.yml | 3 min |
| 2       | Inserting Images with Antora Macros | 4 min |
| 3       | Putting it Together: Basic Structure | 3 min |

### Detailed Steps

1. Open a text editor and examine site.yml to identify where variables are defined (e.g., lab_name attribute)
2. Create a simple AsciiDoc file and reference the lab_name variable using the curly-brace syntax: {lab_name}
3. Verify that the rendered HTML output correctly substitutes the variable value
4. Locate an image file in the images/ directory and note its relative path
5. Insert the image into your AsciiDoc content using the Antora macro format: image::images/filename.png[]
6. Add optional parameters to the image macro such as alt text and width: image::images/filename.png[alt="Description", width=50%]
7. Render the lab content to verify that the image displays correctly with all specified parameters

### Key Takeaways

- AsciiDoc variables are defined in site.yml and referenced in content using curly-brace syntax
- Antora's image macro uses the format `image::path/to/image.png[]` with optional parameters for alt text and sizing
- Variable usage and proper macro syntax enable content reusability and maintainability
- The Antora documentation site builder automatically resolves image paths and variable interpolation during rendering

### Infrastructure Notes

None — this module is entirely about understanding file format syntax and configuration concepts.
