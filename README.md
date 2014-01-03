Agenda
------

These are the lectures I'll give:

* Brief review of some topics covered in EN 600.439/639.
* Introduction to RNA sequencing data analysis
* Introduction to big-data methods for sequencing data analysis
* Project ideas

At the end of the semester, we'll have 2 or 3 class sessions dedicated to final project presentations.  That leaves 19-20 class sessions where we're free to discuss either (a) relevant literature, or (b) project progress.

That's it!  The rest of the discussion is guided, fueled, and led by you.

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
    * Bowtie
    * BWA
* Compression
    * CRAM
    * Quip
* Sketching and streaming
    * eXpress: [Streaming fragment assembly for real-time analysis of sequencing experiments](http://www.nature.com/nmeth/journal/v10/n1/full/nmeth.2251.html) by Roberts, Pachter (also listed above)
* Scalable computing
    * Scalable alignment
        * [CloudBurst: highly sensitive read mapping with MapReduce](http://bioinformatics.oxfordjournals.org/content/25/11/1363.short) by Schatz
    * Scalable indexing
        * [Rapid Parallel Genome Indexing with MapReduce](http://dl.acm.org/citation.cfm?id=1996104) by Menon, Bhat, Schatz
    * Scalable pipelines
        * [Fragment assignment in the cloud with eXpress-D](http://www.biomedcentral.com/1471-2105/14/358/abstract) by Roberts, Feng, Pachter (also listed below)
