<img align=right  src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTyy337olOGg3hXKd-rgf9J-VwbL453qo6eu9qBDagXdfGM2r0g&s">

# Guidance (methods, hints and tips)
This document is for reviewers using Github to assign badges to SE publications.

## F.A.Q: Why use Github? 

We prefer tools like Github over tools like EasyChair, HotCrp, etc., since tools like  Github allows for the collaborative interactive
process required to prepare artifacts for widespread use.

Also, if reviewers create anonymous ids for themselves, then Github easily supports blind review.

## Goal

We say that artifact evaluation is a **collaborative** process where reviewers and authors work together to double check that research
artifacts are ready to be used (or have been used) by other teams.

This is **not** an adversarial  process. 

- Everything we deal with here relates to materials that have passed peer review at other venues.
- Hence we expect a very large "acceptance" rate, i.e., most authors will get the badges that they request.

This is an **interactive** process where reviewers and authors may have multiple interactions, e.g.,

- Reviewers point out some small issue that stops an artifact installing on a new platform.
- Authors fix up their artifacts to remove that issue.

## Actors

The review process described here has three actors:

- Authors who offer submissions;
- Reviewers who review submissions;
- Track chairs who assign submissions to reviewers.

<br clear=all><img   width=400 align=right src="https://i0.wp.com/www.literaryrebel.com/wp-content/uploads/success-formula.jpg?resize=1080%2C628">

## Process for Authors:

1. _Prepare the artifact_: According to  [Wilson et al](https://arxiv.org/pdf/1609.00037.pdf) artifacts can take
               many forms such as simple text files,  checklists to guide questionnaires,  scripts,   packages,   containers, etc.  You should choose an artifact  format that works best for you.
2. _Check out_: check out the repo maintained by the track chairs into your own local branch.
2. _Document_:
     - Authors document their artifact using some files specified by the track chairs. Those files may change from conference to 
       conference and might include:
       - CONFLICTS.md: list of review committee members that are conflicted with the authors (and should not review the
            submission).
       - CONTACTS.md: emails for authors.
       - LICENSE.md: usage permissions.
       - INSTALL.md: where to get the artifact;  how to install it. 
       - STATUS.md: if applying for multiple badges, list those here.
       - README.md: introductory notes on the artifact, and perhaps, tutorials on how to use it.
           [Example1](https://gist.github.com/fvcproductions/1bfc2d4aecb01a834b46). 
           [Example2](https://medium.com/@meakaakka/a-beginners-guide-to-writing-a-kickass-readme-7ac01da88ab3). 
     - Those files are added to a subdirectory of the submissions directory in the repo.
     - Commit those changes (in your branch) back to Github.

3. _Pull request_: issue a pull request to the master branch of the repo.
4. Watch for help requests from authors (in the issue devoted to your submission).
5. Then leave the reviewers alone during their review period. Note that track chairs will delete your comments during this period (so reviewers can reflect on your submission without
   your distractions).
6. Once your submission's issues are labelled _AuthorComment_, feel free to interact extensively with the reviewers.

<br clear=all><img   width=400 align=right src="https://stockx.imgix.net/products/streetwear/Supreme-Directors-Chair-Red.jpg?fit=fill&bg=FFFFFF&w=700&h=500&auto=format,compress&q=90&dpr=2&trim=color&updated_at=1553192445">

## Process for Track chairs:

1. _Recruitment_: gather your review team. Collect anonymous Github ids from each reviewer.
1. _Create repo_: make a public repo. Make with one sub-directory for each badge that might be assigned. 
   -  Those badges may change from conference to conference and might include  the following. 
      - reusable
      - available
      - replicated
      - reproduced
   - For the definitions of the badges above, see [the ICSE'20 artifacts track cfp](https://conf.researchr.org/track/icse-2020/icse-2020-Artifact-Evaluation#Call-for-Submissions).
1. _Define your tracking labels_: these labels will be the process marks that track the stages of the review process. 
   - The labels you use may change from conference to conference and might include the following. Note that the first half shows the process of the artifact through the review process and the last five are final decisions (which are added at the end of the review process):
        - 1. InitialInstalls 
        - 2. NeedsFirstReview
        - 3. NeedsSecondReview
        - 4. AuthorComment
        - nobadge
        - reusable
        - available
        - replicated
        - reproduced              
1. _Watch for pull requests from authors_: ensure that their materials are submitted to unique sub-directory names under the badge directories.
2. _Assignment_:  to assign reviewers to artifacts, create one (and only one) issue per submission. At the top of that issue, add a link to the sub-directory for the artifact.  Assign some reviewers and the authors to the issue.
3. _Monitor_: watch the comment process, stamping out fruitless discussions. 
     - During _InitialInstalls_, allow author/reviewer interaction (so the installs can be debugged). 
     - During _NeedsFirstReview_ and _NeedsSecondReview_, delete any author comments (so reviewers can reflect on their
       submission without author distaction).
     - During _AuthorComment_,  allow author/reviewer interaction (so the artifacts can be improved and, where possible, reviewer issues can be resolved). 
  
  
<br clear=all><img   width=400 align=right src="https://www.amzdiscover.com/blog/wp-content/uploads/2018/07/reviewers.jpg">

## Process for Reviewers:

1. _Create ids_: reviewers create an anonymous Id for themselves and pass that id to the track chairs.
2. _InitialInstalls_: once assigned to an issue, see if you can use the artifact. Use author/reviewer interaction (so the installs can be debugged). 
3. _NeedsReview_: comment on the artifact (perhaps using the [sample comments shown below](#things-to-look-for)). Ignore any author comments (so your can reflect on submissions without author distactions).
 4. _AuthorComment_ : Use author/reviewer interaction (so the artifacts can be improved and, where possible, reviewer issues can be resolved). 


<br clear=all><img   width=400 align=right src="https://www.trustford.co.uk/img/aftersales/hints.jpg">

## Things to Look For

This section comes from Erin Dahlgren's report  [Getting Research Software to Work:
A Case Study on Artifact Evaluation for OOPSLA 2019](https://2019.splashcon.org/getImage/orig/accpub-OOPSLA2019-licensed.pdf) 
and lists some common comments that reviewers make about artifacts. Reviewers may find the following comments useful in their review.

### Common Negative Comments

- Environment
  - _Not enough resources._ Reviewers didn’t have enough physical resources to test the artifact locally in a reasonable amount of time.
  - _Issues with software dependencies._ Reviewers struggled to find and install the right software dependencies, sometimes preventing them from setting up and testing the artifact.
  - _Works in limited environments._ Reviewers had difficulty getting access to proprietary operating systems and running benchmarks locally.
- Format
  - _Issues with VM or container._ Reviewers encountered errors when they tried to setup VMs and containers, or the VMs and containers slowed down the review process.
  - _Problems with docs._ Reviewers encountered typos in instructions, and missing or unclear instructions.
  - _Errors in scripts._ Reviewers wasted time debugging typos and unexpected errors in helper scripts.
  - _Too complicated._ Reviewers struggled to complete complicated instructions to test complicated artifacts.
- Execution
  - _Long running tests._ Reviewers struggled to complete tests that took hours or days.
  - _Issues compiling or running._ Reviewers encountered errors when they tried to compile or run the artifact.
  - _Ignored errors._ Reviewers weren’t confident about artifacts that emitted errors, even if the results produced were correct.
  - _Downloads during execution._ Reviewers spent a long time running test cases that downloaded data on the fly. Reviewers were also worried that such data would not always be available.
 
### Common Positive Comments

- _Self-contained._ Reviewers were enthusiastic about artifacts that required minimal setup and worked seamlessly.
- _Lightweight._ Reviewers benefited from artifacts that required minimal storage space. They also appreciated being able to download small parts of a large artifact.
- _Comprehensive documentation_. Reviewers praised clear, easy to follow documentation that covered most if not all aspects of the artifact.
