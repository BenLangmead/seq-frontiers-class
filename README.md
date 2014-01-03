Agenda
------

I'll give in-class lectures covering:

* Brief review of some topics covered in [EN 600.439/639](https://github.com/BenLangmead/comp-genomics-class)
* Introduction to RNA sequencing data analysis
* Introduction to big-data methods for sequencing data analysis
* Project ideas

Maybe each of these will take one class session.  At the end of the semester, we'll have 2 or 3 class sessions dedicated to final project presentations.  I will also try to have a few guest lecturers come.  More on this as I nail down those dates.

That leaves roughly 16-18 class sessions where we're free to discuss either (a) relevant literature, or (b) project progress.  I am listing relevant literature below.

Readings
--------

If you are taking my class and you have any trouble accessing these resources, please contact me. All of these articles should be easily accessible from the JHU campus or via VPN / library proxy.

### RNA sequencing data analysis

* Surveys (everyone should read these -- don't pick one of these to present in class):
    * [RNA-Seq: a revolutionary tool for transcriptomics](http://www.nature.com/nrg/journal/v10/n1/full/nrg2484.html) by Wang, Gerstein, Snyder
    * [Computational methods for transcriptome annotation and quantification using RNA-seq](http://www.nature.com/nmeth/journal/v8/n6/pdf/nmeth.1613.pdf) by Garber, Grabherr, Guttman and Trapnell
    * [From RNA-seq reads to differential expression results](http://www.biomedcentral.com/content/pdf/gb-2010-11-12-220.pdf) by Oshlack, Robinson, Young

* Spliced alignment
    * QPALMA: [Optimal spliced alignments of short sequence reads](http://bioinformatics.oxfordjournals.org/content/24/16/i174.full.html) by De Bona et al
    * [MapSplice: Accurate mapping of RNA-seq reads for splice junction discovery](http://nar.oxfordjournals.org/content/38/18/e178.full.pdf) by Wang et al
    * [TopHat: discovering splice junctions with RNA-seq](http://bioinformatics.oxfordjournals.org/content/25/9/1105.full.html) by Trapnell, Pachter, Salzberg
    * [TopHat2: accurate alignment of transcriptomes in the presence of insertions, deletions and gene fusions](http://www.biomedcentral.com/content/pdf/gb-2013-14-4-r36.pdf) by Kim et al
    * [STAR: ultrafast universal RNA-seq aligner](http://bioinformatics.oxfordjournals.org/content/29/1/15.short) by Dobin et al

* Assembly
    * Cufflinks: [Transcript assembly and quantification by RNA-Seq reveals unannotated transcripts and isoform switching during cell differentiation](http://www.nature.com/nbt/journal/v28/n5/full/nbt.1621.html) by Trapnell et al
    * CLASS: [CLASS: constrained transcript assembly of RNA-seq reads](http://www.biomedcentral.com/1471-2105/14/S5/S14?utm_source=dlvr.it&utm_medium=tumblr) by Song, Florea
    * Trinity: [Full-length transcriptome assembly from RNA-Seq data without a reference genome](http://www.nature.com/nbt/journal/v29/n7/full/nbt.1883.html) by Grabherr et al
    * PSGInfer: [Inference of alternative splicing from RNA-Seq data with probabilistic splice graphs](http://bioinformatics.oxfordjournals.org/content/29/18/2300.full.html) by LeGault, Dewey

* Scalable methods
    * eXpress: [Streaming fragment assembly for real-time analysis of sequencing experiments](http://www.nature.com/nmeth/journal/v10/n1/full/nmeth.2251.html) by Roberts, Pachter (also listed below)
    * [Fragment assignment in the cloud with eXpress-D](http://www.biomedcentral.com/1471-2105/14/358/abstract) by Roberts, Feng, Pachter (also listed below)
    * [Sailfish: Alignment-free Isoform Quantification from RNA-seq Reads using Lightweight Algorithms](http://arxiv.org/abs/1308.3700) by Patro, Mount, Kingsford

### Big data methods for sequencing data analysis

* Indexing
    * Surveys
        * [Prospects and limitations of full-text index structures in genome analysis](http://nar.oxfordjournals.org/content/40/15/6993) by Vyverman et al
        * [Indexing Methods for Approximate String Matching](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.11.5629&rep=rep1&type=pdf) by Navarro et al
    * Types of indexes
        * Suffix array: [Suffix arrays: a new method for on-line string searches](http://epubs.siam.org/doi/abs/10.1137/0222058) by Manber, Myers
        * Enhanced suffix array: [Replacing suffix trees with enhanced suffix arrays](http://www.sciencedirect.com/science/article/pii/S1570866703000650) by Abouelhoda, Kurtz, Ohlebusch
        * FM index: [Opportunistic data structures with applications](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=892127) by Ferragina, Manzini
    * Sequencing read alignment tools that use the Suffix Array
        * Segemehl: [Fast Mapping of Short Sequences with Mismatches, Insertions and Deletions Using Index Structures](http://dx.plos.org/10.1371/journal.pcbi.1000502) by Hoffmann et al
    * Sequencing read alignment tools that use the FM Index
        * Bowtie: [Ultrafast and memory-efficient alignment of short DNA sequences to the human genome](http://genomebiology.com/2009/10/3/R25) by Langmead et al
        * Bowtie 2: [Fast gapped-read alignment with Bowtie 2](http://www.nature.com/nmeth/journal/v9/n4/full/nmeth.1923.html) by Langmead, Salzberg
        * BWA: [Fast and accurate short read alignment with Burrows–Wheeler transform](http://bioinformatics.oxfordjournals.org/content/25/14/1754.short) by Li, Durbin
        * BWA-SW: [Fast and accurate long-read alignment with Burrows–Wheeler transform](http://bioinformatics.oxfordjournals.org/content/26/5/589.short) by Li, Durbin
        * BWA-MEM: [Aligning sequence reads, clone sequences and assembly contigs with BWA-MEM](http://arxiv.org/abs/1303.3997) by Li
        * GEM: [The GEM mapper: fast, accurate and versatile alignment by filtration](http://www.nature.com/nmeth/journal/v9/n12/abs/nmeth.2221.html) by Marco-Sola et al
* Compression
    * CRAM: [Efficient storage of high throughput DNA sequencing data using reference-based compression](http://nar.oxfordjournals.org/content/40/22/e171.short) by Hsi-Yang Fritz et al
    * Quip: [Compression of next-generation sequencing reads aided by highly efficient de novo assembly](http://nar.oxfordjournals.org/content/40/22/e171.short) by Jones et al
    * [Adaptive reference-free compression of sequence quality scores](http://arxiv.org/abs/1305.0159) by Janin, Rosone, Cox
* Sketching and streaming
    * eXpress: [Streaming fragment assembly for real-time analysis of sequencing experiments](http://www.nature.com/nmeth/journal/v10/n1/full/nmeth.2251.html) by Roberts, Pachter (also listed above)
    * [Similarity Estimation Techniques from Rounding Algorithms](http://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&ved=0CDAQFjAA&url=http%3A%2F%2Fwww.cs.princeton.edu%2Fcourses%2Farchive%2Fspring04%2Fcos598B%2Fbib%2FCharikarEstim.pdf&ei=BOfGUsqtEbawsASgyYCADg&usg=AFQjCNGhjQeAdc2rz3unSSih-ipPDVDZtw&bvm=bv.58187178,d.cWc) by Charikar
    * [A random-permutations-based approach to fast read alignment](http://www.biomedcentral.com/content/pdf/1471-2105-14-S5-S8.pdf?www.nature.com/doifinder/10.1038/ng.437) by Lederman
* Scalable computing
    * Scalable alignment
        * [CloudBurst: highly sensitive read mapping with MapReduce](http://bioinformatics.oxfordjournals.org/content/25/11/1363.short) by Schatz
    * Scalable indexing
        * [Rapid Parallel Genome Indexing with MapReduce](http://dl.acm.org/citation.cfm?id=1996104) by Menon, Bhat, Schatz
    * Scalable pipelines
        * [Searching for SNPs with cloud computing](http://genomebiology.com/2009/10/11/R134) by Langmead et al
        * [Cloud-scale RNA-sequencing differential expression analysis with Myrna](http://genomebiology.com/2010/11/8/R83) by Langmead, Hansen, Leek
        * [ADAM: Genomics Formats and Processing Patterns for Cloud Scale Computing](http://www.eecs.berkeley.edu/Pubs/TechRpts/2013/EECS-2013-207.html) by Massie et al
        * [Fragment assignment in the cloud with eXpress-D](http://www.biomedcentral.com/1471-2105/14/358/abstract) by Roberts, Feng, Pachter (also listed below)
