# MathJax-SVG-Latex-Editor
MathJax + SVG Editor: Single-page web tool for creating academic content. Combines live LaTeX rendering with dynamic, scalable SVG diagram generation using simple JS functions. Designed for NCERT-style black/white graphics. Portable, fast, and ideal for educational content creation.
.
.
.
.
.
MathJax + SVG Interactive Editor

~Overview

The MathJax + SVG Interactive Editor is a minimalist, single-page web application designed for educators, students, and content creators who need to generate clean, professional-grade mathematical content and vector diagrams side-by-side.

This tool functions as a dual-pane editor: allowing users to write descriptive text and LaTeX equations (rendered by MathJax) on one side, and dynamically generate custom, scalable geometric diagrams (using pure JavaScript/SVG) on the other. It is specifically styled to produce NCERT-like diagrams—featuring black lines, minimal styling, and automatic scaling for high-quality output.

~Key Features

Dual Pane Workflow (50/50 Split): Provides a seamless side-by-side editing experience with instant live preview.

LaTeX Rendering (via MathJax): Supports all standard TeX and LaTeX math syntax for beautiful, web-native equation typesetting.

Vector Diagram Generation: Uses embedded JavaScript helper functions (drawLine, drawCircle, drawTriangle, etc.) to generate clean, scalable SVG graphics based on simple coordinate input.

Multi-Diagram Support: Separate multiple diagram code blocks using /// to generate distinct, vertically stacked graphics.

Dynamic Scaling: Diagrams automatically calculate their necessary viewBox and display size based on the content drawn, ensuring everything remains centered, proportionate, and legible.

NCERT Styling: Enforces strict styling rules (black lines, white/transparent fill, precise text sizing) suitable for educational materials and academic papers.

Self-Contained: The entire application runs from a single HTML file, requiring no backend or complex build process, making it highly portable.

~Tech Stack

Frontend: HTML5, CSS3, Vanilla JavaScript

Mathematics Rendering: MathJax 3

Diagrams: Scalable Vector Graphics (SVG) via native DOM manipulation

~How to Use the Editor

Open the File: Download and open the (your file name).html file in any modern web browser.

Input Text & Math: In the left editor pane, write your main text and enclose LaTeX equations with $ for inline math.

Separate Sections: Use the separator %%% to mark the beginning of your diagram code section.

Write Diagram Code: Write JavaScript using the pre-defined helper functions (e.g., drawLine(SVG, x1, y1, x2, y2)).

Separate Diagrams: Use the separator /// to start a new, completely independent SVG diagram.

Instant Preview: The right pane will update instantly with rendered LaTeX and dynamically generated SVG diagrams, which are sized and stacked automatically.

~Available SVG Functions

Function                                   | Purpose
-------------------------------------------|------------------------------------------------
`drawLine(SVG, x1, y1, x2, y2)`            | Draws a straight line segment.
`drawCircle(SVG, cx, cy, r)`               | Draws a circle with center (cx, cy) and radius r.
`drawPoint(SVG, x, y, r)`                  | Draws a small filled circle (point).
`drawText(SVG, text, x, y)`                | Places a label at position (x, y).
`drawTriangle(SVG, x1, y1, x2, y2, x3, y3)`| Draws a closed triangle polygon.
`drawQuadrilateral(...)`                   | Draws a closed four-sided polygon.
`drawPolygon(SVG, "x1,y1 x2,y2 ...")`      | Draws a general closed polygon.
