# slides-examples
Examples for creating slides/presentations

## LaTeX Beamer

## Software

Compile locally using texlive; a good IDE is VSCode with the LaTeX Workshop extension. Another option is to use Overleaf.
Note that videos cannot be embedded and need to be stored alongside the PDF in a relative path.

## Present

Use pympress (https://github.com/Cimbali/pympress) to present. At the moment, auto-starting videos does not work, see https://github.com/Cimbali/pympress/issues/212. Since I prefer all videos to autostart, I use my own fork that auto-starts and mutes all videos, which is available at https://github.com/whoenig/pympress.

### Important keys

* F - full screen
* D - Overview of all slides
* L - enable virtual laserpointer
* S - swap screens

## RevealJs

Develop locally using VSCode and "Run on Save" by "pucelle" extension to run pandoc whenever the markdown file changes. To view the page with live updates, use "Live Server" by "Ritwick Dey" extension.

## Present

* Make sure to generate a *standalone* HTML, since the default one requires internet to load styles etc. This is done by github actions, or by using:

```
./run-pandoc.sh --embed-resources --standalone
```

Note that this will embed all media files including videos, so only the HTML file is needed for presenting.

* There is a presenter mode, but it only works when using the "Live Server" (not when just opening the html file in the browser):

### Important keys

* F - full screen
* S - speaker view (requires live server)
* ESC - slide overview (and ending fullscreen, typically)

## References

* https://github.com/xieby1/markdown_revealjs
* https://gist.github.com/jsoma/629b9564af5b1e7fa62d0a3a0a47c296
* https://gisbers.de/posts/revealjs-pandoc/
* https://github.com/shd101wyy/markdown-preview-enhanced/blob/master/docs/pandoc-bibliographies-and-citations.md