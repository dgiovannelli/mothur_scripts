## A series of scripts that were designed to facilitate our workflow with *mothur* on our server

Donato Giovannelli - 25 Jan 2018

This repository contains few script that we use in our lab to facilitate the our worflow when working with *mothur* on our *polyphemus* server.

#### *mrdna_motur*
A bash file containing a series of step to create a valid *mothur* fasta file and group file starting from the \*-pf.fasta of Mr. DNA sequencing facility. Starting file assumes that the sequences have been alredy demultiplexed, primer and adaptor removed and concatenated into a single fasta formatted file.

Usage: ``mrdna_motur yourfile
``

#### *get_results*
A bash file renaming and zipping together the basic result files from our *mothur* pipeline to facilitate export from the server. The final zip file will contain the .shared .taxonomy .fasta and .biom files. Modify the script to suit your needs.

To use it just run
``get_results
``in the folder containg the *mothur* analysis files.

#### *mothur_polyphemus.batch*
This file contains our standard *mothur* pipeline.
