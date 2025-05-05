# Auto Multiple Choice OMR & Postcorrect Template

[![License: GPL v2+](https://img.shields.io/badge/License-GPL%20v2%2B-blue.svg)](https://www.gnu.org/licenses/gpl-2.0.html)
[![Project Status: Active](https://img.shields.io/badge/status-active-success.svg)]() <!-- Add relevant link if available -->
[![Made with LaTeX](https://img.shields.io/badge/Made%20with-LaTeX-blue.svg)](https://www.latex-project.org/)
<a href="https://www.auto-multiple-choice.net/index.en" target="_blank">
  <img src="https://www.auto-multiple-choice.net/logo.png" alt="Auto Multiple Choice" height="20" style="vertical-align: top;"/>
</a>



This repository provides a ready-to-use Auto Multiple Choice (AMC) template for generating separate OMR answer sheets and post-correction reports.

- **Author:** Rakesh Jana
- **Version:** 1.0.0
- **Date:** May 5, 2025

## Contents

- `separate-postcorrect.tex`  
  LaTeX template for an exam with separate answer sheet and post-correction support.

- `options.xml`  
  AMC project configuration file (defines export formats, document names, project settings).

- (Optional) `students.csv`  
  Sample student list. Make sure to fill this file with actual student details. Also don't change column name.

## Installation

### Packaging the Template

Before installing, package your template files into a compressed archive:
```bash
# From the repository root:
tar czvf omr-postcorrect-template.tgz \
    separate-postcorrect.tex \
    options.xml \
    description.xml \
    students.csv
```

### 1. Via `.tgz` archive

1. Package the files into a `.tgz` (e.g., `omr-postcorrect-template.tgz`).
2. Copy the `.tgz` into your AMC models directory:
   ```bash
   cp omr-postcorrect-template.tgz ~/.AMC.d/Models/
   ```
3. Restart AMC GUI.

### 2. Via AMC GUI

1. Open AMC, go to **Menu → Project → User Templates**.
2. Click **Browse Models Folder**, and paste your `omr-postcorrect-template.tgz` in the opened directory.
3. Restart the GUI; the new template will appear when creating a project.

## Usage

1. In AMC GUI, click **New Project** and select **omr-postcorrect-template** (or the name you gave the `.tgz`).
2. Set exam metadata (title, date, etc.) in the LaTeX file (`separate-postcorrect.tex`).

## Contributing

Contributions are welcome! Please feel free to open an issue to report bugs or suggest features, or submit a pull request with improvements.

## License

This template uses the GNU GPLv2+ license, in line with Auto Multiple Choice. Please retain license headers in all files.
