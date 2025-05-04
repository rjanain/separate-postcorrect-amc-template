# Auto Multiple Choice OMR & Postcorrect Template

This repository provides a ready-to-use Auto Multiple Choice (AMC) template for generating separate OMR answer sheets and post-correction reports.

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

## License

This template uses the GNU GPLv2+ license, in line with Auto Multiple Choice. Please retain license headers in all files.
