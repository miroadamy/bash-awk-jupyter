# Interactive Tutorials for AWK and bash

__A work in process, occasionally worked on.__

There are countless [Awk tutorials](https://www.google.com/search?q=awk+tutorial) online.

Also for bash ... TBD...

I decided to finally teach myself Awk and document the process in [Jupyter notebooks](http://jupyter.org/) with a Bash kernel. This is the result.

## AWK outline

1. [Basics of Awk](Awk-tutorial-01-basics.ipynb)
2. [Built-in Functions](Awk-tutorial-02-built-in-functions.ipynb)
3. [Arrays](Awk-tutorial-03-arrays.ipynb)
4. ...

## bash outline

1. 
2. [bash basics](bash-basics-1.ipynb)
3. Arrays
4. ...


### See also

* sed: "sed is a stream editor. A stream editor is used to perform basic text transformations on an input stream (a file or input from a pipeline)."
** What is the difference between sed and awk?
* miller: "Miller is like sed, awk, cut, join, and sort for name-indexed data such as CSV."
* jq: "jq is like sed for JSON data - you can use it to slice and filter and map and transform structured data with the same ease that sed, awk, grep and friends let you play with text."

## Running the notebooks:

To setup environment, build the Docker image or use mine:

```
docker pull miroadamy/jupyter-docker-bash

or 

docker build -t miroadamy/jupyter-docker-bash .
```

Then run it from working directory. I use non-standard port as I run several other notebooks 

```
docker run --rm -p 9999:8888 -v $(pwd):/home/jovyan/work miroadamy/jupyter-docker-bash:latest
```

Notebook contains GNU awk version

```
awk --version
GNU Awk 4.1.4, API: 1.1 (GNU MPFR 4.0.1, GNU MP 6.1.2)
```
