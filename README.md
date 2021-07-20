# LaTeX Resume to PDF

[![LaTeX Resume to PDF](https://github.com/TakshPSingh/latex-resume-to-pdf/actions/workflows/latex-resume-to-pdf.yml/badge.svg)](https://github.com/TakshPSingh/latex-resume-to-pdf/actions/workflows/latex-resume-to-pdf.yml)

Pipeline to automate the process of converting your latex resume into pdf and releasing it.

## Credits

* [sb2nov/resume](https://github.com/sb2nov/resume) (resume template)
* [softprops/action-gh-release](https://github.com/softprops/action-gh-release)
* [xu-cheng/latex-action](https://github.com/xu-cheng/latex-action)

## User Guide

* Fork this repo, clone it, rename your_name.tex, edit it, commit your changes, and push.
* Simply pushing your changes won't trigger the pdf render process. This is by design, to prevent unnecessary renders for minor changes.
* Once you've made enough changes to warrant a new release, run the following commands:
  * git tag v* (for example git tag v2.0)
  * git push origin v*
 * This will trigger a GitHub action defined in latex-resume-to-pdf.yml, which will convert your resume into pdf and release it.
 * You can go to the releases section of your repo for a detailed look into your pdf render history.
 * But if you want a permalink to your latest pdf resume (that you could maybe use in your personal website or job applications), it should be similar to the following:
 
> https://github.com/TakshPSingh/latex-resume-to-pdf/releases/latest/download/your_name.pdf

## Why?

* Tracking resume iterations is difficult without a version control system like Git.
* In my opinion, it's cleaner to use GitHub releases to seperate raw latex files and rendered pdfs.
* You get a nice permalink to your latest resume ([example](https://github.com/TakshPSingh/latex-resume-to-pdf/releases/latest/download/your_name.pdf)).
* Automation is cool.
