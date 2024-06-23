# Actuarial Exam Problem Archive

## Introduction
Welcome to my Actuarial Exam Problem Archive. This repository contains a collection of actuarial exam problems and solutions that I've compiled over several years for use in my teaching. These materials were created whenever I needed specific problems for my courses, and they have accumulated over time. While they provide valuable practice for various actuarial exams, they are not intended to demonstrate the evolution of the exams or to be representative of any specific trends.

## Project Purpose
The primary objective of this project is visibility. By sharing this extensive archive, I aim to help colleagues and future actuaries in their study and preparation. Additionally, this project showcases my ability to organize and present complex information clearly, reflecting my skills in teaching, leadership, and teamwork.

## Functionality
This project leverages LaTeX for document preparation, with custom macros for streamlined formatting and solution visibility:
- `\JGWitem{}`: Custom macro for listing exam problems. It can be easily adjusted to include problem sources, page breaks, or other formatting.
- `\showsol{}`: Custom macro for displaying solutions, which can be toggled for different audiences (e.g., instructors or students).

### Key Features:
- **Modular Design**: Problems and solutions are stored in individual files, allowing for easy compilation and customization.
- **Dynamic Formatting**: Custom macros provide flexibility in presentation, enabling tailored documents for various stakeholders.

## Examples

### Example 1: Including Multiple Problems
Here’s a snippet demonstrating how to include multiple problems using the `\input` command:

```latex
\documentclass{article}
\textheight=9.5in
\textwidth=6.25in
\hoffset=-0.75in
\voffset=-0.5in

\input{../../macros_lifecon}

\newcommand{\showsol}[1]{#1}
\newcommand{\JGWitem}[1]{\item \textbf{#1}}

\begin{document}
\begin{enumerate}
    \input{C3May2007_24.tex}
    \input{C3Nov2000_8.tex}
    \input{C3May2005_31.tex}
    \input{C3May2005_40.tex}
\end{enumerate}
\end{document}
