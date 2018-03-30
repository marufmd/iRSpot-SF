# iRSpot-SF
Prediction of Recombination Hotspots using Sequence Based Features
## Installation
No installation needed. Just download the files in a folder or download the iRSpot-SF-master.tar.gz file and extract it into your loacal directory. Following prerequisites are required to run the software.

1. Install python 3.4 or latest version
2. Install following python packages:
    - numpy
    - pandas
    - sklearn
        
## Run the software:
**Step 1:** Go to the folder "input". Open the text file "input.txt". Enter the DNA query sequence in FASTA format.

Example of a DNA sequence in FASTA format:

    >YDL087C 1.67     
    ATGTCAACTATGTCAACGCCTGCCGCAGAACAACGCAAACTCGTCGAACAGCTGATGGGCAGGAC 
    TTCAGTTTCCGCCACAACAGGTATTCGCATCAAAAAAGAGACCTCGGACTACACGATCCAAGATC 
    TGCAAGTCATACCTTGTTGGCGAGTGCCCCTACGACCTGTTTCAGGGCACCAACAGAGCCTGGGA 
    AAATGCCCGCAGATGCATCTTACCAAGCATAAAATTCAGTACGAGAGAGGGTCAAGCAGGGCAAA 
    ACGTTTCCCGAATTCGAAAGAGAATATCTGGCCATTCTATCTCGGTTGTTAATGAGTGTAATGGC 
    CAGATATCCGTAGCACTACAAAATCTAAAACACACCGCTGAGAACGAATGAAGATTCAGCAGGTT 
    ACCGAAGAACTAGATGTCTTGGACGTGCGGATAGGCCAATGGGACAAGAGATTGATTCTTTAATT 
    CGTGCAGATGAAGTCAGTATGGGTATGCTACAGCAGTCAAATTACAAGAACTGATTAGTAAAAGG 
    AAAGAAGTTGCAAAACGTGTACGAAACATACAGAAAACGTGGGCCAGAGCGCCCAGCAAAAGTTA 
    CAGGTTTGCGAGGTGTGTGGGGCATCCTATCGCGTTTAGATACAGACAGAAGGCTTGCTGACCAC 
    TTCTTGGGGAAGATTCATCTGGATATGTCAAGATGAGAGAGGATTATGATCGGCTAATGAAGAAT 
    AACCGGACAACTAACGCAGCAAGACAGCTACTACACTACCCGGAAGACGCTTTGTGTA

**Step 2:** Type the following command in the terminal:

    $ python  model.py
    
**Step 3:** Go to the folder "output". Open the text file "output.txt". It will show you the prediction for the DNA query sequence of "input.txt". *HOT* is shown for HOTSPOT and *COLD* for COLDSPOT. For the sample DNA sequence it'll show:

    HOT
    
**N.B., If the DNA sequence is not in FASTA format, it will not predict anything.**
