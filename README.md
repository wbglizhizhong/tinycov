### tinycov

Tinycov is a small standalone command line utility written in python to plot the coverage of a BAM file quickly.
This software was inspired by [Matt Edwards' genome coverage plotter](https://github.com/matted/genome_coverage_plotter).


### Installation

git clone https://github.com/cmdoret/tinycov.git

> TODO: Distribute as a package on Pypi

### Usage

Usage: tinycov.py [OPTIONS] BAM

Options:
  -r, --res INTEGER     Size of windows in which to compute coverage, in
                        basepairs.  [default: 10000]
  -s, --skip INTEGER    Stride between windows, in basepairs.  [default: 1000]
  -n, --name TEXT       Name of the sample (plot title). Base name of input
                        file by default
  -b, --blacklist TEXT  Exclude those chromosomes from the plot. List of
                        comma-separated chromosome names.
  -w, --whitelist TEXT  Only include those chromosomes in the plot. List of
                        comma-separated chromosome names.
  -o, --out PATH        Output file where to write the plot. If not provided,
                        the plot is shown interactively
  -t, --text PATH       Output file where to write the raw data table.
  -p, --ploidy INTEGER  Ploidy of input sample, used to estimate coverage
                        threshold for aneuploidies
  --help                Show this message and exit.
