# Haplocheck
[![Build Status](https://travis-ci.org/genepi/haplocheck.svg?branch=master)](https://travis-ci.org/genepi/haplocheck)

Haplocheck is a software that leverages the mitochondrial phylogeny to detect contamination in mtDNA sequencing studies. By generating in-silico mixtures and reassessing the 1000 Genomes data, we also show the practicability of our approach for contamination detection in whole genome sequencing studies. We provide haplocheck as a standalone pipeline and as a cloud web service (via https://mitoverse.i-med.ac.at). 

## Run Haplocheck locally

Using Cloudgene, the complete workflow can also be executed locally. The final HTML report is located at `<out-folder>/report`. Haplocheck requires Java 8 or higher.

        curl -s install.cloudgene.io | bash -s 2.0.0-rc14
        ./cloudgene install https://github.com/genepi/haplocheck/releases/download/v1.0.5/haplocheck.zip
        ./cloudgene run haplocheck@1.0.5 --files <input-files> --output <out-folder>  

## Run Haplocheck as a cloud service

Haplocheck is a contamination tool using the mtDNA phylogeny and has been integrated into the [mitoverse](https://mitoverse.i-med.ac.at) mtDNA platform based on [Cloudgene](https://www.cloudgene.io). 

## Haplocheck Documentation
Documentation can be found [here](https://mitoverse.readthedocs.io/en/latest).

## Testdata
The 1000 Genomes Phase3 file analyzed with mutserve can be found [here](https://github.com/genepi/haplocheck/raw/master/test-data/contamination/1000G/all/1000g-nobaq.vcf.gz). 

## Blog
Check out our [blog](http://haplogrep.uibk.ac.at/blog/) regarding mtDNA topics.

## Contact
[Hansi Weissensteiner](mailto:hansi.weissensteiner@i-med.ac.at) ([@haansi](https://twitter.com/whansi)) and [Sebastian Schoenherr](mailto:sebastian.schoenherr@i-med.ac.at) ([@seppinho](https://twitter.com/seppinho)); Institute of Genetic Epidemiology, Medical University of Innsbruck;
