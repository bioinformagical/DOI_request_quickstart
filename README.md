# CyVerse Data Commons DOI Request Quickstart Repo

You should import this repo to build CyVerse Quickstarts

**See this quickstart [rendered on ReadTheDocs](https://cyverse-cyverse-quickstart-template.readthedocs-hosted.com/en/latest/)**

## What this repo contains

|Item|Description|Notes|
|----|-----------|-----|
|index.rst|Home page for documentation. Before you being.|documents written in markdown will need to be converted to restructured text|
|step2.rst|Organize the dataset in the CyVerse Data Store|
|step3.rst|Add metadata to the dataset top folder|
|step4.rst|Submit the request for the DOI and wait for validation|
|step5.rst|After data are published|
|/img (folder)|Images for the tutorials|CyVerse logos and other useful images are already here|
|example_directives_delete.rst|Example page with code for common restructured text objects||
|cyverse_rst_defined_substitutions.txt|restructured text substitutions for common URLs and images||
|conf.py|Place to add tutorial and author name;versioning||
|README.md|This page||
|/slides (folder)|Slides associated with the tutorial here|version controlled files preferred, PPT acceptable|
|/misc (folder)|miscellaneous needed for building documentation| |
|License.md|License|this license file applies to all materials created by CyVerse for this documentation|
|Contributors_maintainers.md|Contact information and recognition||


## Simple contribution instructions

### Reporting an error or issue via GitHub

- Click the 'issues' tab at the top of this GitHub page to let us know about a
  simple mistake such as a typo or missing file.

 OR

- Send an email to [Tutorials@CyVerse.org](mailto:tutorials@cyverse.org)

## More complex contributions

### Fixing and/or improving documentation via GitHub

1. [Fork](https://help.github.com/articles/fork-a-repo/) this repo to your
   GitHub account
2. Make edits directly to the **index.rst** file. Edits may be made to the fork
   the web interface to your GitHub account or
   [clone](https://help.github.com/articles/cloning-a-repository/) the repo to
   work on your local computer. For very significant changes (we suggest
   [making a new branch](https://help.github.com/articles/creating-and-deleting-branches-within-your-repository/)).
3. Commit change; if working from a local copy, push those changes to your fork
   in Github.
4. Submit a pull request back to the master repository; you may need to act on
   feedback before your request is merged.





### Procedure
(This section to be removed)

2. Edit the **index.rst**. Save images or other files in the appropriate
   directories. **See our recommended style guide for writing documentation below.**
3. Since tutorials will likely span multiple pages, you can copy internal pages
   page as many times as needed. Update the table of contents at the top of the
   'index.rst' accordingly. We will have **only one tutorial or quick start per repo.**
4. Save your work:
    - individual pages (e.g. *'index.rst, step2.rst'*)
    - images (as *'.png'* files in the  the *'img'* folder)
    - changes or additions to *'cyverse_rst_defined_substitutions.txt'*
5. Edit the *'conf.py'* file to set the project and author information
6. Build the tutorial:

        $ make html
7. Your HTML site will be in the _build directory that has been created (you can
   preview this in your web browser at this time).
8. Commit your changes and push the tutorial back to GitHub.
9. Notify [Tutorials@CyVerse.org](mailto:Tutorials@CyVerse.org) that your
   tutorial is ready for inclusion in the main CyVerse documentation repo.
   We will review and verify the contribution, and add you as a maintainer repo
   in the CyVerse collection. You should make future edits following the
   instructions above for 'Fixing and/or improving documentation via GitHub.'
   Alternatively, you can host your tutorial independently on ReadTheDocs
   following their [instructions for importing documentation](https://docs.readthedocs.io/en/latest/getting_started.html#import-your-docs).
   We will also follow up about ensuring test data associated with the
   documentation are available and open.

### Documentation Style Guide

*General Principles*

- Write instructions in short numbered steps
- Where possible limit step to one action; small final actions such as
  'press submit' should be separated by a semicolon
- Limit the use of screenshots; where they are needed, use ReStructured text
  directives for [substitution of images](http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html#substitution-definitions)
- Use the *'raw ::html'* directive to enter hyperlinks so that they will open
  in a new tab. See each repo for an example of the code
- Example data associated with documentation should be anonymously available on
  CyVerse Data Commons (Tutorials@cyverse.org can help you with this)
- Discovery Environment applications should be directly linked to documentation
  (clicking the 'info' button on any application will give you the 'App URL')
- Atmosphere images should be directly linked to documentation
  (e.g. "atmo.cyverse.org/application/images/####"

*Specific examples*

|Instruction|Example|
|-----------|-------|
|Steps generally begin with a verb or preposition|<ul><li>Click on the button<li>Under the "Result" menu</ul>|
|Locations of files are given in absolute paths|<ul><li>/dir1/dir2/file.extension</ul>|
|Top-level menus in Discovery Environment Apps in double quotes|<ul><li>Under "Input" select...</ul>|
|Subheadings/steps in Discovery Environment Apps in single quotes|<ul><li>For 'sensitivity' enter...</ul>|
|Buttons and keywords in bold|<ul><li>Click on **Apps**<li>Select **Arabidopsis**<li>Set 'sensitivity' to **Medium**</ul>|
