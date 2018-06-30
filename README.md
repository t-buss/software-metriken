# Software metrics as an indicator for security vulnerabilities

Seminar paper on detecting security vulnerabilities using software metrics

TeX-Style based on [LNCS](https://www.springer.com/de/it-informatik/lncs/conference-proceedings-guidelines)

## Building with Docker

If you are like me and do not want to install a whole lot of LaTeX packages, you can compile the document using Aergus' LaTeX image like this:

`docker run --rm -it -v $PWD:/doc aergus/latex sh -c "cd /doc && pdflatex -interaction batchmode document.tex"`

This will take a long time on the first try, as Docker needs to download the 4Gb large image from Docher Hub. Subsequent builds will be lightning fast though.
When you no longer need to build the image, you can simply delete the Docker image to free some disk space: `docker rmi aergus/latex`
