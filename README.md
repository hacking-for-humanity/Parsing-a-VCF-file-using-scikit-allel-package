# Parsing-a-VCF-file-using-scikit-allel-package
Parsing the VCF file using the scikit-allel package and extracting the desired data lines

* Read the VCF file 
with open('sample.vcf', mode='r') as vcf:
    print(vcf.read())

*Import scikit-allel package

Install using pip install scikit-allel 

or 

conda install -c conda-forge scikit-allel

1) import and read read the file into callset collection using allel.read_vcf()

2) Parse the file based on white spaces, colons and commas with regex package.

3) Select the gene of interest using the gene ID's referred back to NCBI gene database or Filter = PASS column in file.

4) Keep parsing until we have our required values to work with and load them into a dictonary. 
