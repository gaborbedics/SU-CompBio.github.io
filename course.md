---
layout: page
title: PhD Course
permalink: /course/
---

## General information

Lecture outlines, recommended reading material and other information for the PhD
course at Semmelweis University, titled "Adatelemzés és programozás orvos
biológusoknak I". This semester, the course will be in hungarian, but these
notes are in english.

The course builds heavily on the [Carpentries
Foundation](https://carpentries.org/) material and teaching philosophy. It is
intended for beginners, with no or very little programming knowledge.

**Location**: Histology Seminar Room (ground floor), Semmelweis University,
1<sup>st</sup> Department of Pathology and Experimental Cancer Research, H-1085
Budapest, Üllői út 26.

**Time**: every Wednesday, from 16:30 to 18:00, starting with the 4<sup>th</sup>
of September.

**Requirements**: participants must bring a laptop with a Mac, Linux, or Windows
operating system (not a tablet, Chromebook, etc.) that they have administrative
privileges on. They are also required to abide by the [Carpentries Code of
Conduct](https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html).

**Grading and homeworks**: there are going to be 12 short homework exercises (no
homework for Week 1 and Week 8), where you will be asked to think about a
problem, try to solve it, and most importantly, document your thoughts, the
issues or problems you ran into. You will need to submit one or a few small text
files, tables, documents, or scripts through Dropbox File Requests. We are going
to discuss solutions and issues next week. You will need to submit at least 6 of
them to pass, and 10 for excellent. Keep in mind that you are here to
learn and try things out. Active participation, discussing issues and asking
questions is much more important, than submitting perfectly written programming
exercises.

**Contact**: send and email to sebestyen.endre at med dot semmelweis-univ dot hu
if you have any questions or comments.

**Teachers**: Endre Sebestyén, Bence Szalai, Gábor Turu, Miklós Cserző

## Week 1 - 4<sup>th</sup> of September - Endre Sebestyén

*Introduction, software installation, getting around in R and RStudio.*

[Presentation]({{ site.url }}/assets/phd_course/eloadas_2019-09-04.pdf)

Delivery plan:

- Explain content of course
- Explain Code of Conduct
- Explain name labels
- Explain stickies and feedback
- Homeworks and grading
- Short introduction from everybody
- R and RStudio download and setup
- Getting started with R and RStudio
- Discussing *your own* data and analysis plans

### R and RStudio installation

We will use the R programming language, RStudio, and command line tools during
the semester that need to be set up first. Right now, we will install R and
Rstudio.

If you run into issues: [Common configuration problems and
solutions](https://github.com/carpentries/workshop-template/wiki/Configuration-Problems-and-Solutions)

[R](https://www.r-project.org/) is a programming language that is especially
powerful for data exploration, visualization, and statistical analysis. To
interact with R, we use [RStudio](https://www.rstudio.com/).

#### Windows

[Video tutorial](https://www.youtube.com/watch?v=q0PjTAylwoU)

Install R by downloading and running
[this](https://cran.r-project.org/bin/windows/base/release.htm) .exe file from
[CRAN](https://cran.r-project.org/index.html). Also, please install the [RStudio
IDE](https://www.rstudio.com/products/rstudio/download/#download). Note that if
you have separate user and admin accounts, you should run the installers as
administrator (right-click on .exe file and select "Run as administrator"
instead of double-clicking). Otherwise problems may occur later, for example
when installing R packages.

#### macOS

[Video Tutorial](https://www.youtube.com/watch?v=5-ly3kyxwEg)

Install R by downloading and running
[this](https://cran.r-project.org/bin/macosx/R-latest.pkg) .pkg file from
[CRAN](https://cran.r-project.org/index.html).  Also, please install the
[RStudio IDE](https://www.rstudio.com/products/rstudio/download/#download).

#### Linux

You can download the binary files for your distribution from
[CRAN](https://cran.r-project.org/index.html). Or you can use your package
manager (e.g. for Debian/Ubuntu run `sudo apt-get install r-base` and for Fedora
run `sudo dnf install R`).  Also, please install the [RStudio
IDE](https://www.rstudio.com/products/rstudio/download/#download).

### Getting around in R and RStudio

We will base our R/RStudio lessons on the Data Carpentry [Data Analysis and
Visualization in R for Ecologists](https://datacarpentry.org/R-ecology-lesson/)
lessons. Take a look at the main page and the [Before we
start](https://datacarpentry.org/R-ecology-lesson/00-before-we-start.html)
section.

## Week 2 - 11<sup>th</sup> of September - Endre Sebestyén

*Data organization and cleanup, structuring projects, tidy data*

Delivery plan:

- Recap of basic organizational stuff for newcomers
- Short introduction from everybody
- Checking R, RStudio, LibreOffice/Excel setup
- Discussing data organization in spreadsheets
- Recommended readings
- Homework explanation

### Data organization in spreadsheets

Before diving into the details of R and RStudio, we will discuss data
organization in spreadsheets. Most researchers use spreadsheets to collect data,
and this is the start of every analysis. However, computers need data to be
organized in a particular way. They can't recognize typos, colored excel lines
and other things that are easy to interpret and/or correct by humans.

We will use the Data Carpentry lesson titled [Data Organization in Spreadsheets
for Ecologists](https://datacarpentry.org/spreadsheet-ecology-lesson/) to learn
about these things.

- [Introduction](https://datacarpentry.org/spreadsheet-ecology-lesson/00-intro/index.html) and
  [data formatting](https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data/index.html)
- [Common formatting problems](https://datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes/index.html)
- [Dates as data](https://datacarpentry.org/spreadsheet-ecology-lesson/03-dates-as-data/index.html)
- [Quality control](https://datacarpentry.org/spreadsheet-ecology-lesson/04-quality-control/index.html)
- [Exporting data](https://datacarpentry.org/spreadsheet-ecology-lesson/05-exporting-data/index.html)

You will need some kind of spreadsheet software for this, like Microsoft Excel
or LibreOffice. To setup LibreOffice, check the details
[here](https://datacarpentry.org/spreadsheet-ecology-lesson//setup.html).

### Recommended readings

These are some of the papers that describe basic data organization principles,
how to manage projects, etc.

- Tidy Data [10.18637/jss.v059.i10](http://dx.doi.org/10.18637/jss.v059.i10):
  how to organize your data in a clean, easy to handle way.
- A quick guide to organizing computational biology projects
  [10.1371/journal.pcbi.1000424](http://dx.doi.org/10.1371/journal.pcbi.1000424):
  how to organize any project, not just computational biology projects. Anyway,
  [all biology is computational
  biology](http://dx.doi.org/10.1371/journal.pbio.2002050), right?
- Good enough practices in scientific computing
  [10.1371/journal.pcbi.1005510](http://dx.doi.org/10.1371/journal.pcbi.1005510):
  a set of good computing practices, that every researcher can adopt, regardless
  of current level of computational skills.
- Best Practices for Scientific Computing
  [10.1371/journal.pbio.1001745](http://dx.doi.org/10.1371/journal.pbio.1001745):
  a more detailed explanation on how to organize stuff, write code, plan your
  project, collaborate and so on.

### Homework

*Send an email from the address you would like to use for getting the
homework submission link.* Homework deadline is 23:00, 15<sup>th</sup> of
September. We will discuss them next week.

Think about what we learned today about organizing data in spreadsheets, tidy
data and your own project, datasets and analysis plans. Keeping all of this in
mind, *create a single spreadsheet* showing how you would organize your
experimental data. Add columns as needed, and include a few rows with example
data. You can also add some explanations or comments in the table.

What kind of data will you collect? Clinical information, gene expression
values, genetic information, something else? Is it categorical or continuous?
How many observations, patients or experiments are you planning? Are you
planning to do multiple measurements on the same sample? Is it important to
record experimental setup, machine parameters? What happens if you have missing
data, for example no clinical information, or the experiment failed for a
certain sample?

## Week 3 - 18<sup>th</sup> of September - Endre Sebestyén

*Intro to R I: variables, vectors, lists, functions*

## Week 4 - 25<sup>th</sup> of September - Endre Sebestyén

*Intro to R II: subsetting and missing data*

## Week 5 - 2<sup>nd</sup> of October - Endre Sebestyén

*Intro to R III: reading in and writing out data, factors, data frames*

## Week 6 - 9<sup>th</sup> of October - Endre Sebestyén

*Intro to R IV: CRAN and Bioconductor, using dplyr*

## Week 7 - 16<sup>th</sup> of October - Endre Sebestyén

*R graphics: data visualization with ggplot2, R Markdown*

## Week 8 - 30<sup>th</sup> of October - Endre Sebestyén

*The Linux/UNIX operating systems and the command line*

*Recap of R and RStudio, Q & A session*

## Week 9 - 6<sup>th</sup> of November - Gábor Turu

*Command line I: file system, creating, deleting, editing and looking at files*

## Week 10 - 13<sup>th</sup> of November - Endre Sebestyén

*Command line II: manipulating, filtering, rearranging files, shell scripts*

## Week 11 - 20<sup>th</sup> of November - Endre Sebestyén

*Version control: git and github*

## Week 12 - 27<sup>th</sup> of November - Bence Szalai

*Intro to python I: basic syntax, Jupyter development environment*

## Week 13 - 4<sup>th</sup> of December - Bence Szalai

*Intro to python II: variable types*

## Week 14 - 11<sup>th</sup> of December - Bence Szalai

*Intro to python III: conditional statements, loops, functions*
