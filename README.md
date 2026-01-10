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

## Instructor Workflow

### Creating and Publishing Materials

1. **Edit in private repo**: Create/edit markdown files in main TCE432 repository (private)
   - Draft, revise, and finalize all content there
   - Keep all working drafts, notes, and planning materials private

2. **Convert final drafts to PDF**: 
   ```bash
   pandoc file.md -o file.pdf --pdf-engine=xelatex
   ```

3. **Copy ONLY finalized PDFs to public repo**:
   ```bash
   cp "file.pdf" "/path/to/TCE432-Materials/Week XX - Name/Materials/"
   ```
   - ⚠️ **IMPORTANT**: Only publish student-ready, finalized materials
   - Do NOT copy drafts, planning docs, or works-in-progress
   - Public repo = final, polished, student-facing materials only

4. **Commit and push**:
   ```bash
   cd "/path/to/TCE432-Materials"
   git add -A
   git commit -m "Add/update Week XX materials"
   git push origin main
   ```

5. **Canvas links auto-update**: HTML pages with GitHub raw URLs automatically serve updated content

### Updating Existing Materials

When revising materials mid-semester:
1. Edit markdown in private repo
2. Convert updated version to PDF
3. Overwrite the existing PDF in public repo (same filename)
4. Commit and push - links update automatically

### Key Principles

- **Private repo (TCE432)**: All planning, drafts, notes, markdown sources
- **Public repo (TCE432-Materials)**: Only final, student-ready PDFs and images
- **Separation ensures**: Course planning stays private while materials remain accessible

## GitHub Raw URL Format

`https://raw.githubusercontent.com/OhioMathTeacher/TCE432-Materials/main/Week%20XX/Materials/filename.pdf`

*Note: Spaces in paths must be URL-encoded as `%20`*
