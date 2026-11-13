# priya-project1-sequence-analysis
NGS sequence analysis assessment 

**NGS DATA MUTATION IDENTIFICATION** 

The program compares DNA sequence reads against an established reference sequence to identify, record and analyse base mutations. This is to address whether the genotoxic agent used for the treated group significantly impacts mutation patterns.

**Running the Program**

Open the link to the google colab notebook and either click run all function or manually run each cell in order to ensure all variables, reads and functions are defined before the final analysis.

**Inputs and outputs**
The programme uses the reference sequence to validate read sequences, identify and analyse mutations as well as calculate significance. Outputs include sample information such as ID, group, errors, mutations, as well as reporting valid/invalid reads, subsitution counts, and mismatch percentages. Final statistical output include welch's t test and a p-value. 

**Code design**: 

I divided work into functions rather than one long piece of code to make the code less repetitive and more concise - making it easier to read and to identify where bugs occurred.

In my functions I used if/else so my code could identify valid and invalid reads and then follow different decisions based off the condition (e.g. ensuring only valid data was analysed - so to prevent any crashes). "Continue" also could have been used to skip invalid reads but i felt if/else was more familiar to me and easier to understand when reading the code. 

I also used dictionaries instead of lists to store my results from my functions. This meant I could retrieve data more easily that using indexes or slices. It also meant I could format my output better. 

**Testing**:

I tested each program with different types of data inputs against a short reference ("ATGC") to simplify the results. I checked that empty inputs resulted in an empty input and i inputted reads that were valid as well as invalid using wrong lengths, characters, and both errors together to test how the programme dealt with them. I used assert so I could see if the output was what i was expecting to see. 
