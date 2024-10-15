---
permalink: /
title: "Zhifei Hu 胡知非"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
\documentclass{article}
\usepackage{geometry}
\geometry{a4paper, margin=1in}
\usepackage{amsmath}

\usepackage{graphicx}
\usepackage{enumitem} % for customizing itemize
\usepackage{multicol} % for two-column layout
\usepackage{hyperref}


I am currently an Algorithm engineer at Speedbot Robotics Co., Ltd.[Speedbot](https://www.speedbot.com/en/home) since 2023. Prior to that,  I completed a 3-year MS in Optical Engineering at Fudan University, Shanghai, China, under the supervision of Prof. Min Xu and Prof. Xiangchang Zhang. 

Publication
======
Like many other Jekyll-based GitHub Pages templates, Academic Pages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Project
======
\vspace{-0.5em}\hrule\vspace{0.7em}
\begin{itemize}[left=0pt, itemsep=0.1em, parsep=0em]
    \item \textbf{Fast Measurement of Surface Topographies Using a Phase-Measuring Deflectometric Microscopy}[MATLAB] \hfill June 2020 -- June 2023 \\
    \textit{Lead Researcher} \\
    \vspace{-1.5em}
    \begin{itemize}[left=0pt, itemsep=0.05em, parsep=0em]
        \item[-] \textbf{Objective:} Implement a deflectometric microscope system from 0 to 1 to semiquantitatively measure surface defects for in-situ applications. 
        \item[-] \textbf{Methods:}
            \begin{itemize}[left=0pt, itemsep=0.05em, parsep=0em]
                \item[-] Designed a pinhole camera model to release precise focusing requirements.
                \item[-] Achieved defect reconstruction using a path integral reconstruction algorithm combined with sparse representation.
            \end{itemize}
        \item[-] \textbf{Outcome:} Research findings were published in the IEEE Photonics Journal.
    \end{itemize}
\end{itemize}
\begin{itemize}[left=0pt, itemsep=0.05em, parsep=0em]
 \item \href{https://www.youtube.com/watch?v=yxMVsodcq9g}{PaintPro Paint Defect Detection System }[OpenCV][C++]\hfill June 2023 -- July 2024 \\
    \vspace{-1.5em}
    \begin{itemize}[left=0pt, itemsep=0.05em, parsep=0em]
        \item[-] \textbf{Objective:} Develop a 3D camera based on Phase Measuring Deflectometry, specifically designed to capture mirror-like and quasi-mirror-like images.
        \item[-] \textbf{Methods:}
            \begin{itemize}[left=0pt, itemsep=0.05em, parsep=0em]
                \item[-] Developed a geometric calibration model using a markerless flat mirror and the Levenberg–Marquardt algorithm.
                \item[-] Implemented paint surface reconstruction through Multiple View Geometry and the Particle Swarm Optimization (PSO) algorithm.
            \end{itemize}
        \item[-] \textbf{Outcome:} The project was put into production at the Geely plant in Hunan, China.
    \end{itemize}
\end{itemize}

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
