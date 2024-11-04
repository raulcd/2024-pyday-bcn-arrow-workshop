# 2024-pyday-bcn-arrow-workshop
Apache Arrow Workshop for PyDay Barcelona 2024


# A deep dive into the Arrow Columnar format with pyarrow and nanoarrow

Apache Arrow has become a de-facto standard for efficient in-memory columnar data representation. You might have heard about Arrow or using Arrow, but do you understand the format and why it's so useful? This tutorial will dive deep into the details of the Arrow columnar format, the different types and buffer layouts, and explore those details interactively using the pyarrow and nanoarrow libraries.

## Setup

To run this tutorial locally, follow those steps:

**Clone this repository**

    git clone https://github.com/raulcd/2024-pyday-bcn-arrow-workshop.git

**Install the necessary packages**

The code examples require numpy, pyarrow and [nanoarrow](https://github.com/apache/arrow-nanoarrow), and JupyterLab (or alternative) to run the notebooks:

    pip install jupyterlab numpy pandas pyarrow nanoarrow

We recommend to create an environment, either with conda/mamba:

    conda create -n arrow-tutorial python numpy pandas jupyterlab
    conda activate arrow-tutorial
    python -m pip install pyarrow nanoarrow

or create a virtual environment:

    cd 2024-pyday-bcn-arrow-workshop
    python -m venv .venv
    source .venv/bin/activate
    pip install jupyterlab numpy pandas pyarrow nanoarrow

**Launch Jupyter**

From the repo directory:

    jupyter lab
