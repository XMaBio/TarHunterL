===============================================================================
         TarHunterL: a tool for predicting miRNA target 
                and target mimics (eTM) in plants.
===============================================================================

Version 1.0

Author: Xuan Ma <skyxma@tjnu.edu.cn>
 
This program is free software: you can redistribute it and/or modify it under the 
terms of the GNU General Public License as published by the Free Software 
Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY 
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
PARTICULAR PURPOSE. See the GNU General Public License for more details.




===============================================================================
                                  Description
===============================================================================
TarHunterL is a lightweight TarHunter. It does not has cross-species
conservation filter.  TarHunterL is performed in the following two steps:

(i)  Search miRNA targets using FASTA;
(ii) Parse FASTA result to obtain miRNA targets and eTMs.


Citation: Ma X. et al. TarHunter, a tool for predicting conserved microRNA 
targets and target mimics in plants. Bioinformatics. 2018 May 1

===============================================================================
                                 Prerequisites
===============================================================================
OS Platform: Linux
Perl 5.10, or above

Executables under PATH:
FASTA        (fasta36, http://faculty.virginia.edu/wrpearson/fasta/fasta36/)




===============================================================================
                                   Examples
===============================================================================

cd test/

A. Target prediction with score cutoff of 4

    perl ../TarHunterL.pl -q mir.fa -b targ.fa -o out1 -f 4

B. eTM prediction

    perl ../TarHunterL.pl -q mir.fa -b targ.fa -o out2 -I




===============================================================================
                                   Notes
===============================================================================
The script has been tested on a Fedora (release 16) server with Perl v5.14.3, 
 and on a UBUNTU (release 14.04) PC with Perl v5.18.2.

