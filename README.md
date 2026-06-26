# Polygon-Design
The style design page for Polygon Design
A fully offline design system and local Figma plugin for creating websites, landing pages, software interfaces, and reusable product components in the Polygon Interactive visual style.

The project combines:

An editable offline HTML design system
A local Figma plugin that generates editable design-system layers
Reusable colour, typography, button, tab, card, form, landing-page, and software-shell patterns
An embedded Roman Clay material texture
CSS, JSON, and customised HTML export tools
Design language

Polygon Interactive uses a refined, tactile visual system built around warm neutrals, softened blues, deep structural tones, and restrained brass detailing.

Core palette
Token	Value	Intended use
Ivory	#F5F0E6	Primary page and application background
Light Grey	#D9DCDF	Clean neutral surfaces and dividers
Roman Clay	Embedded image texture	Feature banners, presentation panels, and tactile backgrounds
Dark Grey	#596069	Secondary text and subdued interface elements
Charcoal	#262B31	Primary text, navigation, and structural surfaces
Pale Blue	#DCEBF4	Tabs, secondary actions, and calm interface states
French Blue	#739FBE	Standard actions and active navigation states
Navy Blue	#17324F	Confirmation, submission, and high-importance actions
Brass	#B08D57	Decorative rules, icons, and premium detailing
Brass Ink	#3F2F20	Text displayed on French Blue surfaces
Typography
Role	Typeface
Titles and headings	Fraunces
UI and body copy	Inter
Labels, code, and data	JetBrains Mono

Fallback fonts are included when the preferred fonts are not available locally.

Interaction rules
Buttons
French Blue is used for standard actions.
Pale Blue is used for secondary actions and heading tabs.
Navy Blue is reserved for confirmation, save, submit, and completion actions.
Brass is a decorative accent and should not be used as the default action colour.
Text on French Blue uses the dark brass-brown #3F2F20.
Roman Clay

Roman Clay is treated as a distinct material rather than a variation of Light Grey.

Use it selectively for:

Feature banners
Presentation panels
Quiet section backgrounds
Premium content blocks

Avoid using it behind dense tables, long-form content, or complex data displays.

Project structure
.
├── manifest.json
├── code.js
├── README.md
└── source
    ├── polygon_interactive_offline_design_system_v4.html
    └── roman_clay.png
Figma plugin

The included local Figma plugin creates an editable Polygon Interactive design-system page containing:

Local colour styles
Local text styles
Button components
Active and inactive tabs
Form fields
Cards and status components
A landing-page pattern
A software dashboard pattern
Editable Roman Clay material panels
Fraunces, Inter, and JetBrains Mono typography roles
Install the plugin
Clone or download this repository.
Open the Figma desktop application.
Open any Figma Design file.
Go to Plugins → Development → Import plugin from manifest.
Select manifest.json.
Open a blank Figma Design file.
Run Polygon Interactive Design System Builder from the Development plugins menu.

The plugin will generate the complete design-system page as editable Figma layers.

Create a .fig file

Figma's .fig format is proprietary and is created by Figma itself.

After running the plugin:

Review or edit the generated design system.
Use Figma's local-save or export workflow.
Save the file as a .fig file from within Figma.
Offline HTML design system

The HTML design system is stored in:

source/polygon_interactive_offline_design_system_v4.html

Open it directly in a modern browser. No web server, package manager, build step, or internet connection is required.

HTML features
Live colour-token editing
Editable text mode
Local browser persistence
Light and dark preview modes
CSS token export
JSON token export
Customised HTML export
Embedded Roman Clay image
Responsive landing-page and software-interface examples
Local font requirements

For the closest visual match, install:

Fraunces
Inter
JetBrains Mono

The project does not distribute font files. This keeps the repository lightweight and avoids font-licensing issues.

When a preferred font is unavailable, the HTML and Figma plugin use compatible fallback fonts.

Development

The Figma plugin uses plain JavaScript and does not require a build process.

Edit the plugin
Update code.js.
Return to Figma.
Reload the development plugin.
Run it again in a blank file.
Edit the HTML system

The editable design tokens are defined near the beginning of the HTML file as CSS custom properties:

:root {
  --ivory: #f5f0e6;
  --light-grey: #d9dcdf;
  --dark-grey: #596069;
  --charcoal: #262b31;
  --pale-blue: #dcebf4;
  --french-blue: #739fbe;
  --navy: #17324f;
  --brass: #b08d57;
  --brass-ink: #3f2f20;
}

The typography roles are:

--display: "Fraunces", Georgia, "Times New Roman", serif;
--body: "Inter", ui-sans-serif, sans-serif;
--mono: "JetBrains Mono", "SFMono-Regular", Consolas, monospace;
Recommended workflow
Use the HTML file to review and refine design tokens.
Export updated CSS or JSON tokens.
Run the Figma plugin to generate editable design-system assets.
Build page and software concepts from the generated components.
Save the completed Figma file as a .fig file.
Apply exported tokens to production web or software projects.
Browser support

The offline HTML system is intended for current versions of:

Chrome
Edge
Firefox
Safari

Some visual effects, including backdrop-filter and color-mix(), may render differently in older browsers.

Contributing

Contributions should preserve the established Polygon Interactive design principles:

Warm, tactile surfaces
Clear hierarchy
Restrained use of decorative colour
Strong accessibility contrast
Consistent typography roles
Practical components for websites and software
Fully editable and reusable source assets

Before submitting changes, verify both the offline HTML system and the generated Figma output.
