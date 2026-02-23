# Chapter 4 — Results and Discussion

This repository contains the LaTeX source for **Chapter 4** of the dissertation.

## Repository Structure

```
├── chapter4.tex      # Main LaTeX source for Chapter 4
├── references.bib    # BibTeX bibliography file
├── figures/           # Directory for figures and images
└── README.md
```

## How to Use

### Writing

Open `chapter4.tex` and replace the `% TODO` comments with your content. The document is organised into the following sections:

1. **Introduction** – overview of the chapter and restatement of research questions.
2. **Data Overview** – description of the dataset and data-collection process.
3. **Descriptive Statistics** – summary statistics, tables, and figures.
4. **Results** – main findings organised by research question (add or remove subsections as needed).
5. **Discussion** – interpretation, comparison with literature, and implications.
6. **Summary** – key takeaways and transition to the next chapter.

### Adding References

Add BibTeX entries to `references.bib` and cite them in the text with `\citep{}` or `\citet{}`.

### Adding Figures

Place image files in the `figures/` directory and include them with:

```latex
\begin{figure}[H]
  \centering
  \includegraphics[width=0.8\textwidth]{figures/your-figure.png}
  \caption{Your caption here.}
  \label{fig:your-label}
\end{figure}
```

### Compiling the Document

```bash
pdflatex chapter4.tex
bibtex chapter4
pdflatex chapter4.tex
pdflatex chapter4.tex
```

Or, if you have **latexmk** installed:

```bash
latexmk -pdf chapter4.tex
```