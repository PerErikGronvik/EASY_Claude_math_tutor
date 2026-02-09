# Recuirements
- Python 3.10+
- Jupyter Notebook
- VS Code with Python and Jupyter extensions
- `uv` package manager (install with `pip install uv`) (setup file helps you with this, it will propmt you to install it if you don't have it)

# Mathematical Concept Notebooks

Interactive Jupyter notebooks for university-level mathematics courses (Calculus 1-4, Statistics, AI, Data Science) designed to work with GitHub Copilot in VS Code. We recommend using Claude Sonnet 4.5 or newer as your Copilot model for the best experience. For free ones, I think GPT 4.1 is the best as of 09.02.2026.

## What This Is

This project provides a structured environment for learning mathematics through code with AI assistance. GitHub Copilot is configured to:
- Explain mathematical concepts step-by-step
- Create interactive visualizations
- Guide you through problem-solving at your own pace
- Keep notebook structure organized

## Example Usage

Open a notebook (e.g., `3k/3d_lagrange_ellipse_problems.ipynb`) and ask Copilot questions like:

**You:** "What is a partial derivative and how do I visualize it?"

**Copilot will:**
1. Add your question as a markdown cell
2. Explain the concept clearly
3. Create code demonstrations with plots
4. Wait for your next question instead of jumping ahead

This creates a natural back-and-forth learning experience where you control the pace.

## Quick Start

1. **Clone this repository**
2. **Copy the AUTO_JUPYTER_IN_VS_CODE Create a course folder** 
3. **Run setup:**
   - Edit `example.pyproject.toml` - remove # to add packages or add # to remove packages.
   - Rename it to `pyproject.toml`
   -  `.\setup.ps1` (Windows) or `./setup.sh` (Linux/Mac)
4. In the folde create a file. yoursubject.ipynb
5. **Reload VS Code** and select the kernel inside the notebook
6. **Start asking Copilot questions** in your notebook
7. **change .github/copilot-instructions.md to change Copilot's behaviour

## Project Structure

```
.
├── .github/                    # AI assistant configuration
│   └── copilot-instructions.md # How Copilot should interact with notebooks
├── 3k/                         # Calculus 3 (Matte 3000) notebook example
├── RenameFolderAndRunSetup/    # Template for creating new course folders
│   ├── setup.ps1               # Windows setup script (creates a .venv in the folder and makes it reachable for jupyter in vs code.)
│   ├── setup.sh                # Linux/Mac setup script
│   ├── pyproject.toml          # Base project config
│   └── example.pyproject.toml  # Annotated package reference
└── missing_packages.md         # Track missing dependencies
```

## Contributing & Reporting Issues

**Found a missing package dependency?** Add it to `missing_packages.md` or contact **PerErikGronvik**.

**Want to add a new course?** Copy the `RenameFolderAndRunSetup/` template, rename it, and customize the packages.

## License

MIT License - See [LICENSE](LICENSE) file.

Free to use, copy, distribute, and modify. Attribution appreciated!

## Credits

Created by Per Erik Grønvik for mathematics students using AI-assisted learning.
