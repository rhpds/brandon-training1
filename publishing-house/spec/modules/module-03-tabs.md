# Module 03: Tabs

### Brief Overview

This module covers UI tab configuration in Showroom environments. Participants learn how tabs provide learners with quick access to terminals, external links, and documentation. The module explains tab properties including name, type (terminal or external link), port/path for internal services, URL for external links, and the external flag that controls link behavior. Participants understand how to configure each tab type and validate that tabs work correctly in the rendered Showroom UI.

### Audience and Time

- **Target personas:** Lab authors, Showroom configuration specialists, environment designers
- **Prerequisites for this module:** Understanding of Antora configuration from Module 2; familiarity with tab concepts in web UIs
- **Estimated duration:** 10 minutes

### Learning Objectives

- Configure terminal and external link tabs in Showroom UI environments using proper YAML properties
- Distinguish between internal service tabs (using path/port) and external link tabs (using url parameter)
- Validate tab configuration and understand how the external flag controls whether links open in new tabs or the same window

### Lab Structure

| Section | Title | Duration |
|---------|-------|----------|
| 1       | Tab Types and Properties | 3 min |
| 2       | Terminal vs. External Link Tabs | 3 min |
| 3       | Configuration Validation and Testing | 4 min |

### Detailed Steps

1. Open ui-config.yml and locate the tabs configuration section
2. Identify tab properties: name (display label), type (terminal or external-link), and url or path
3. Examine a terminal tab example: type should be "terminal" with port and path properties pointing to an internal service
4. Observe that terminal type uses port (e.g., 8080) and path (e.g., /app) to construct the internal service URL
5. Examine an external link tab example: type should be "external-link" with url property containing the full external URL
6. Check the external property (true/false) to understand link behavior: true opens in new tab/window, false opens in current window
7. Add a new tab entry with all required properties: name, type, and either (path/port) for terminal or url for external link
8. Validate YAML syntax using a YAML linter and check that the Showroom preview renders the tabs correctly
9. Click each tab in the preview to verify it navigates to the correct destination

### Key Takeaways

- Tabs in Showroom are configured as a list in ui-config.yml with properties for name, type, and endpoint
- Terminal tabs require type, port, and path; external tabs require type and url
- The external property determines whether external links open in a new window or replace the current page
- Proper YAML indentation and property names are essential for tabs to render correctly
- Tab configuration can be tested quickly in the Showroom preview without full infrastructure provisioning
- Different tab types serve different purposes: terminals for command-line access, external links for resources outside the lab environment

### Infrastructure Notes

Terminal tabs require that the Showroom environment has a running service accessible on the specified port. External link tabs have no infrastructure requirements — they can reference any publicly accessible URL.
