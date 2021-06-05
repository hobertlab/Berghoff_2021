# Circuit Transcription Factors

This repository contains code to analyze transcription factor
expression patterns in C. elegans, from which we generate a list
of putative circuit transcription factors. See Berghoff et al., 2020.

## Usage

### Prerequisites

You should have the R programming language installed with the "gtools" package.

### Inputs

herm\_full\_edgelist_090618.csv - Connectome edgelist of adult
hermaphrodite, retreived from [wormwiring.org](http://wormwiring.org) 

non\_somatic\_neurons.csv - Self-generated list of non-somatic neurons

non\_somatic\_neurons\_classes.csv - Same as above, just grouped by class

tfs\_expression\_binary.csv - All complete expression patterns of
transcription factors in C. elegans

tfs\_expression\_classes\_binary.csv - Same as above, just grouped by class

tf\_gene\_names.csv - List of transcription factor names, derived from
tfs\_expression\_binary.csv 

### Outputs

all\_tfs.csv - Analysis of all provided transcription factors

all\_significant\_tfs.csv - Analysis of transcription factors with
corrected p-value < 0.05. This is the list of putative circuit
transcription factors.
