# Writing tutorials for Neuromatch Academy (NMA)

Thank you for agreeing to write tutorials for NMA! We're so glad you're here. We try to smooth out writing tutorials so you can concentrate on doing what you do best. 

## Environment

Tutorials need to be writen in python in the Google Colab environment.
Students will use Google Colab to run the tutorials (unless Colab is unavailable in their country) to reduce setup req./library dependencies issues and provide enough compute power for resource intensive tutorials (e.g. deep learning tutorials).

## Tutorial structure

There will be 4 tutorials per day. Each tutorial aims to be short and concise (15-20 minutes max.), it is therefore essential to limit the amount of text and code present on-screen to the bare minimum required for understanding. We want students to focus on understanding the core concepts of the course, rather than focusing on data manipulation, plotting, etc. The rule of thumb is that students will need to write *3 lines of code per tutorial*.

## Organization & Communication

As a content creator, you create the python tutorials. You will need to coordinate with the day organizer so the tutorials meet the objectives of the day (see shared google drive: NMA > curriculum & content > Content creator role.doc) (https://docs.google.com/document/d/1EqDdBy3KPnK0B9ronMhPwa_WnJDjnKIK_fPs9jrDiUY)

Tutorials can take anywhere between 1-2 weeks to prepare, so start as early as possible! Here is how to proceed:

1. Read the 1-pagers for the tutorials you are in charge of: (shared google drive: NMA > curriculum & content > One-pare Topic/ Lecture summaries/)
2. Meet with the day organizer to discuss the tutorial lecture content and what students will be asked to do in tutorials. At this stage it will be essential to decide what you want each exercise of each tutorial to do.
3. You familiarize yourself with existing tutorial templates to understand the format of [NMA tutorials](https://github.com/NeuromatchAcademy/course-content/tree/master/tutorials)
4. Start with the coding of the tutorials (Only when you have finalised step 2! otherwise you'll have to redo a bunch of tutorials!)
   - This is important to minimise the amount of adjustment and doing/redoing required at a later stage. Iterating over step 2 in much detail is much more efficient than: creating code, then deleting whole exercises/tutorials and recoding new ones from scratch) if there is a mismatch.
5 - Reiterate and refine 4 for small adjustments.

## Structure of tutorials

Using markdown headings (#, ##, ###, etc.) can be used to automatically create headings for tutorials, objectives, and exercises, respectively. Use `---` in markdown to separate different exercises/sections.

Example tutorials are available at [NMA github course-content/tutorials](https://github.com/NeuromatchAcademy/course-content/tree/master/tutorials).

For each tutorial:
1. Import all necessary libraries, plotting settings and plotting functions in the top code cell of the tutorial
        - write `# @title` at the top of the cell, and click `...`>`Form`>`Hide code` to hide the code cell (special colab trickery)
2. Describe the tutorial objectives using 2-3 sentences + bullet points
3. Split the tutorial into 2-4 exercises. Each exercise should have:
   - A short description of what we want the student to do in this exercise
   - All equations necessary to implement the computation req. in the exercise (incl. links to external papers/websites for further reading)
   - A detailed itemized list called `Suggestions` (bullet point list) of the itemized actions we want the students to perform to complete the exercise
   - Code skeleton including all the plotting function req. for completing the exercise (incl. complete [PEP8 compliant](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) docstrings)
   - (optional) Include hints in the code skeletton to highlight where the students should complete the code and what python functions they could use to complete it (e.g.: '#Hint: use the function `np.exp()` to exponentiate' )
   - (optional) A sample output of what the correct output of the exercise should look like. In order to prevent students from focussing on reproducing exactly the plots/expected-outputs rather than understanding the core concepts, we provide them with the plotting functions, and use XKCD style for the expected sample outputs.
4. Create sample answers for each tutorial, and so that the technical team can check the tutorials, and to facillitate training for the TAs prior to the summer school.

## Reviewing

* Tutorials need to be approved by day organizer before submitting them to the [NMA course-content github repo](https://github.com/NeuromatchAcademy/course-content/)
* Once approved, submit all tutorials to [NMA github tutorials](https://github.com/NeuromatchAcademy/course-content/tree/master/tutorials) by June 5th so that the technical team can test the tutorials and check for standardization across all NMA tutorials.
* This is [the tutorial reviewing guide](https://github.com/NeuromatchAcademy/course-content/blob/master/tutorials/reviewing-tutorials.md). We try to minimize the burden on the tutorial authors. You're the stars! 
* [We use a branch-pull-request workflow for content](https://guides.github.com/introduction/flow/). You stage everything on your own branch - you can mess up this branch as much as you want, it's 100% yours. Then when you're ready, you create a pull request to ask to merge your branch with the master branch (the stuff everybody sees). Add Marco and Patrick as reviewers. They'll review your notebooks, make comments, and after a couple of iterations they will merge onto master.
