---
permalink: /
title: "Zhifei Hu 胡知非"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


I am currently an Algorithm engineer at Speedbot Robotics Co., Ltd.[Speedbot](https://www.speedbot.com/en/home) since 2023. Prior to that,  I completed a 3-year MS in Optical Engineering at Fudan University, Shanghai, China, under the supervision of Prof. Min Xu and Prof. Xiangchang Zhang. 

Publications
======
- **Z. Hu**, X. Zhang, W. Lang, Y. Chen, T. Chen, and M. Xu, "Fast Measurement of Surface Topographies Using a Phase-Measuring Deflectometric Microscopy," in *IEEE Photonics Journal*, vol. 15, no. 2, pp. 1-7, April 2023, doi: [10.1109/JPHOT.2023.3243736](https://doi.org/10.1109/JPHOT.2023.3243736).  

- W. Lang, X. Zhang, Y. Chen, T. Chen, **Z. Hu**, and X. Jiang, "A General Reconstruction Framework for Deflectometric Measurement Based on Nonuniform B-Splines," in *IEEE Transactions on Instrumentation and Measurement*, vol. 72, pp. 1-11, 2023, Art no. 5015511, doi: [10.1109/TIM.2023.3279466](https://doi.org/10.1109/TIM.2023.3279466).


Projects
======
- **Fast Measurement of Surface Topographies Using a Phase-Measuring Deflectometric Microscopy** [MATLAB]  
  _Lead Researcher_  
  June 2020 – June 2023  
  - **Objective:** Implement a deflectometric microscope system from scratch to semiquantitatively measure surface defects for in-situ applications.
  - **Methods:**  
    - Designed a pinhole camera model to ease precise focusing requirements.
    - Achieved defect reconstruction using a path integral reconstruction algorithm combined with sparse representation.
  - **Outcome:** Research findings were published in the IEEE Photonics Journal.

- [PaintPro Paint Defect Detection System](https://www.youtube.com/watch?v=yxMVsodcq9g) [OpenCV][C++]  
  June 2023 – July 2024  
  - **Objective:** Develop a 3D camera based on Phase Measuring Deflectometry, specifically designed to capture mirror-like and quasi-mirror-like surfaces.
  - **Methods:**  
    - Developed a geometric calibration model using a markerless flat mirror and the Levenberg–Marquardt algorithm.
    - Implemented paint surface reconstruction through Multiple View Geometry and the Particle Swarm Optimization (PSO) algorithm.
  - **Outcome:** The project was put into production at the Geely plant in Hunan, China.

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
