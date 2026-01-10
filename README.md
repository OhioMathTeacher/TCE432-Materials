# TCE 432/532 Course Materials

Student-facing materials for TCE 432/532 (Methods: Middle & High School Math & Science) - Spring 2026

This repository contains PDFs and resources linked directly from Canvas course pages.

## Repository Structure

```
Week 01 - Teaching Identity/
Week 02 - Analyzing Inquiry Tasks/
    Materials/
        10 Dimensions of Inquiry - Student Handout.pdf
        Promising Lessons (LOW)/ - 6 content-agnostic lessons with inquiry potential
        Full Inquiry Lessons (HIGH)/ - 6 fully revised high-inquiry versions
Week 03 - Redesigning Lessons/
Week 04 - Assessment & Field Prep/
    Materials/ - Assessment protocols, worksheets, field guides
    Student Work (NAEP)/ - Authentic student response samples
Week 08-15/ - Additional weekly materials
```

## Usage

**Students:** Click links from Canvas - files will display directly in your browser as PDFs.

**Instructor Workflow:**
1. Edit markdown files in main TCE432 repository (private)
2. Convert to PDF: `pandoc file.md -o file.pdf --pdf-engine=xelatex`
3. Copy PDFs to appropriate week folder in this public repository
4. Commit and push: `git add -A && git commit -m "..." && git push origin main`
5. Canvas HTML pages with GitHub raw URLs automatically serve updated content

## GitHub Raw URL Format

`https://raw.githubusercontent.com/OhioMathTeacher/TCE432-Materials/main/Week%20XX/Materials/filename.pdf`

*Note: Spaces in paths must be URL-encoded as `%20`*
