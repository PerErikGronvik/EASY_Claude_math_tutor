# Mathematical Concept Notebooks

Interactive Jupyter notebooks for university-level mathematics courses (Calculus 1-4, Statistics, AI, Data Science) designed to work with Claude AI as a coding assistant.

## What This Is

This project provides a structured environment for learning mathematics through code with AI assistance. Claude is configured to:
- Explain mathematical concepts step-by-step
- Create interactive visualizations
- Guide you through problem-solving at your own pace
- Keep notebook structure organized

## Example Usage

Open a notebook (e.g., `3k/3d_lagrange_ellipse_problems.ipynb`) and ask Claude questions like:

**You:** "What is a partial derivative and how do I visualize it?"

**Claude will:**
1. Add your question as a markdown cell
2. Explain the concept clearly
3. Create code demonstrations with plots
4. Wait for your next question instead of jumping ahead

This creates a natural back-and-forth learning experience where you control the pace.

## Quick Start

1. **Clone this repository**
2. **Navigate to a course folder** (e.g., `3k` for Calculus 3)
3. **Check if setup files exist:**
   - If `setup.ps1`/`setup.sh` and `pyproject.toml` exist, run the setup script
   - Otherwise, copy from `RenameFolderAndRunSetup/` template
4. **Run setup:** `.\setup.ps1` (Windows) or `./setup.sh` (Linux/Mac)
5. **Reload VS Code** and select the kernel
6. **Start asking Claude questions** in your notebook

See individual folder READMEs for detailed setup instructions.

## Project Structure

```
.
├── .claude/               # AI assistant configuration
│   └── instructions.md    # How Claude should interact with notebooks
├── 3k/                    # Calculus 3 (Matte 3000) notebooks
├── RenameFolderAndRunSetup/  # Template for new course folders
│   ├── setup.ps1          # Windows setup script
│   ├── setup.sh           # Linux/Mac setup script
│   ├── pyproject.toml     # Base project config
│   └── example.pyproject.toml  # Annotated package reference
└── missing_packages.md    # Track missing dependencies
```

## Contributing & Reporting Issues

**Found a missing package dependency?** Add it to `missing_packages.md` or contact **PerErikGronvik**.

**Want to add a new course?** Copy the `RenameFolderAndRunSetup/` template, rename it, and customize the packages.

## License

MIT License - See [LICENSE](LICENSE) file.

Free to use, copy, distribute, and modify. Attribution appreciated!

## Credits

Created by Per Erik Grønvik for mathematics students using AI-assisted learning.
