
# Part 1 - Brainstorm: Statistics

## Distributions
## Statistical Models
## Methods for Estimation
## Methods for Hypothesis Testing

# Part 2 - Brainstorm: Technologies in Biology

## Microarray
## ...

## In-class exercise 1 (15 minutes)

### Technologies: 

```{r}
techs <- c("microarray", "rna-seq", "dna-seq", 
           "bisulphite-seq", "cytometry", "mass-spec", 
           "10x-chromium", "oxford-nanopore")

s <- sample(length(techs))
data.frame(row=s, techs)
```

### Task: 
#### produce a 2-3 point summary of "how it works"
#### links to a few (<5) good resources
#### create a markdown file for it and upload to README.me in "group assignment" repo

# Part 3 - Brainstorm: Applications in genomics 

# Part 4 - Brainstorm: Linking Technologies to Applications to Statistics

## e.g., microarray -> gene expression -> normally distributed (log intensities)

# Part 5 - Brainstorm: Methods/algorithms in genomics associated to Computer Science

# Part 6 - Pick a "technology" (from above, from [1] or otherwise) to briefly describe

## Exercise 2 (in groups of 1-3): 
### Goal: 
#### write ~2 sentences about what the method does
#### again, make the link (technology -> application -> statistics)
#### list the github usernames of everyone in your group
#### submit a pull request to brainstorm_modified.md


### Users
Ainesh Sewak - asewak

### Technology: HELP-seq
The HpaII tiny fragment- Enrichment by Ligation-mediated PCR (HELP) assay is a means of screening DNA methylation status at a large proportion of cytosine sites through-out the genome. The HELP assay positively identifies hypomethylated loci by means of the HpaII representation. [2]

### Application
* To discover loci with altered copy number with high resolution, sensitivity and accuracy on a single microarray
* Cancer research - testing DNA for cytosine methylation and copy-number variation with limited starting material
* Detect allelic differences in methylation
* Find repetitive sequences
* Detect small events in HpaII fragments
* Human genome sequencing

### Statistics
Using circular binary segmentation for finding change-points. Change-points correspond to positions where the underlying DNA copy number has changed. Therefore, change-points can be used to identify regions of gained and lost copy number.

Circular binary segmentation (CBS) is a modification of the traditional binary segmentation procedure (likelihood ratio statistic), which cannot detect a small change buried in the middle of a large segment of DNA. The key difference is that CBS allows for both a single change and the epidemic alternative.


[1] [https://liorpachter.wordpress.com/seq/](https://liorpachter.wordpress.com/seq/)
[2] [High-resolution genome-wide cytosine methylation profiling with simultaneous copy number analysis and optimization for limited cell numbers] (https://academic.oup.com/nar/article-abstract/37/12/3829/1044056)



