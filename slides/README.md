# TARAN SLIDES: README

## Overview

This repository contains the LaTeX Beamer slides for the presentation titled **"The Walls and the Dark Silicon Era: An Arithmetic Perspective"** by Louis Ledoux. The presentation provides insights into modern challenges faced by computer architects, such as the memory wall, power wall, and dark silicon, focusing on software and hardware solutions to address arithmetic architecture and numerical requirements.

## How to Compile

To compile the slides from the source file:

```bash
pdflatex main.tex
```

Ensure that you have a LaTeX distribution installed that includes the Beamer package.

## Notes for Speaker (Presenter Mode)

The slides contain hidden notes that can be used during the presentation. These notes are attached to individual frames in Beamer and can be viewed on a secondary screen for presenter reference. To enable this:

1. Uncomment the line in the LaTeX source file:

   ```latex
   \setbeameroption{show notes on second screen=right}
   ```

2. Use a dual-screen setup to display the speaker notes on one screen while presenting the main slides on the other.

3. Add speaker notes to each frame using the following syntax:

   ```latex
   \note[item]{Your speaker notes here}
   ```

For more details on setting up Beamer notes, see [this guide](https://gist.github.com/andrejbauer/ac361549ac2186be0cdb).

## Recommended Tool: Pympress

To present with speaker notes effectively, you can use **Pympress**, a modern dual-screen PDF reader designed for presentations. It allows you to display the main slides on one screen and the notes on another.

You can download Pympress from [its GitHub repository](https://github.com/Cimbali/pympress).

## Requirements

- **LaTeX Distribution**: Ensure `pdflatex` and Beamer are available.
- **Python Package**: Install Pympress for speaker notes.
- **Dual-Screen Setup**: Necessary for displaying notes alongside the main presentation.

## Presentation Abstract

The presentation addresses persistent challenges in computer architecture, particularly focusing on arithmetic design in the context of HPC. Topics include:
- Addressing the memory wall, power wall, and dark silicon.
- Trade-offs between precision and energy efficiency, as well as parallelism versus latency for SIMD/vector operations.
- Exploration of custom arithmetic ASIC flows and MLIR to improve design flexibility and efficiency.

## Contact

**Louis Ledoux**
*Department of Computer Architecture, Barcelona Supercomputing Center (BSC), Universitat Politècnica de Catalunya (UPC)*
December 2nd, 2024
