my_ldhot
========

Detect recombination hotspots using population genetic data.

Installation
============

After downloading, switch to the download folder and type 'make'.

Usage
=====

./my_ldhot --seq <seq_file> --loc <loc_file> --lk <lk_file> --res <res_file> --nsim 1000 --out <output_prefix>
./my_ldhot_summary --res <res_file> --hot <hotspot_file> --out <output_prefix>

The seq_file, loc_file, lk_file, and res_file are all derived from LDhat.

my_ldhot produces an output file of the form <output_prefix>.hotspots.txt. This file contains the details of
the windows tested for the presence of a hotspot. This file can be treated as the final product, or 
further summarized using the my_ldhot_summary program. This program uses the output of my_ldhot in conjunction
with the recombination rate estimates to find hotspot boundaries. 