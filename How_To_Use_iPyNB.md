# Instructions on opening ipy notebooks
To set paths, start ipy local server, and open interactive web interface type
```
source pyenv_paths.sh
ipython notebook --pylab inline
```
into terminal (Ubuntu 14.04).

To open existing file in viewer (opens as static web page, great for sharing) type
```
google-chrome http://nbviewer.ipython.org/ &
``` 
into terminal (Ubuntu 14.04). Replace google-chrome with preferred browser of choice.

# Instructions on converting ipy nbs to html/latex/pdf
--html--
```
ipython nbconvert notebook.ipynb --to html --template full
```
--latex--
```
ipython nbconvert notebook.ipynb --to latex --template article
```

--latex then to pdf--
```
ipython nbconvert notebook.ipynb --to latex --template article --post PDF
```

--to slides--
```
ipython nbconvert notebook.ipynb --to slides
```