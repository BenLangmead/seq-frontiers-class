Class sessions
--------------

At the beginning of class, I will lead some informal discussions covering:

* Introduction to geonmics, computational genomics, and DNA sequencing
* Introduction to RNA sequencing data analysis
* Introduction to big-data methods for sequencing data analysis
* Project ideas

You'll give a work-in-progress presentation on your final project sometime around spring break.  You'll give a final project presentation at the end of the semester.  A couple guest lectures are likely as well.

Otherwise, class sessions will be devoted to discussing literature.  A student will be selected ahead of time to present in each class, and the student will select and announce 1 or 2 papers for discussion.  The student will then lead a 60-to-75-minute discussion of those papers in class.  The student should present the main ideas and results of the paper using some combination of slides, chalkboard, and demonstrations.  Everyone is encouraged to participate in every discussion; participation is an important part of your grade.

Readings
--------

If you are taking my class and you have any trouble accessing these resources, please contact me. All of these articles should be easily accessible from the JHU campus or via [VPN](http://portalcontent.johnshopkins.edu/sslvpn/JHConnect-FAQ.html) / [library proxy](http://old.library.jhu.edu/services/computing/proxyfaqs.html).

### Broad surveys

* [Life and its Molecules](http://www.aaai.org/ojs/index.php/aimagazine/article/viewArticle/1744) by Lawrence Hunter
* [A decade's perspective on DNA sequencing technology](http://www.nature.com/nature/journal/v470/n7333/abs/nature09796.html) by Elaine Mardis
* [Sequencing technologies -- the next generation](http://www.nature.com/nrg/journal/v11/n1/abs/nrg2626.html) by MichaelMetzker
* [The DNA Data Deluge](http://spectrum.ieee.org/biomedical/devices/the-dna-data-deluge) by Schatz, Langmead

### RNA sequencing data analysis

* Surveys
    * [RNA-Seq: a revolutionary tool for transcriptomics](http://www.nature.com/nrg/journal/v10/n1/full/nrg2484.html) by Wang, Gerstein, Snyder
    * [RNA sequencing: advances, challenges and opportunities](http://www.nature.com/nrg/journal/v12/n2/full/nrg2934.html) by Ozsolak, Milos
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

* Comparisons
    * [Systematic evaluation of spliced alignment programs for RNA-seq data](http://www.nature.com/nmeth/journal/v10/n12/full/nmeth.2722.html) by Engstrom et al
    * [Assessment of transcript reconstruction methods for RNA-seq](http://www.nature.com/nmeth/journal/v10/n12/full/nmeth.2714.html) by Steijger et al

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
        * [A practical algorithm for finding maximal exact matches in large sequence datasets using sparse suffix arrays](http://bioinformatics.oxfordjournals.org/content/25/13/1609.short) by Khan et al

    * Sequencing read alignment tools that use the FM Index
        * Bowtie: [Ultrafast and memory-efficient alignment of short DNA sequences to the human genome](http://genomebiology.com/2009/10/3/R25) by Langmead et al
        * Bowtie 2: [Fast gapped-read alignment with Bowtie 2](http://www.nature.com/nmeth/journal/v9/n4/full/nmeth.1923.html) by Langmead, Salzberg
        * BWA: [Fast and accurate short read alignment with Burrows–Wheeler transform](http://bioinformatics.oxfordjournals.org/content/25/14/1754.short) by Li, Durbin
        * BWA-SW: [Fast and accurate long-read alignment with Burrows–Wheeler transform](http://bioinformatics.oxfordjournals.org/content/26/5/589.short) by Li, Durbin
        * BWA-MEM: [Aligning sequence reads, clone sequences and assembly contigs with BWA-MEM](http://arxiv.org/abs/1303.3997) by Li
        * GEM: [The GEM mapper: fast, accurate and versatile alignment by filtration](http://www.nature.com/nmeth/journal/v9/n12/abs/nmeth.2221.html) by Marco-Sola et al

    * Indexing and querying large collections of sequencing reads using a suffix array and/or FM Index
        * Gk-array: [Querying large read collections in main memory: a versatile data structure](http://www.biomedcentral.com/1471-2105/12/242) by Philippe et al
        * [CRAC: an integrated approach to the analysis of RNA-seq reads](http://genomebiology.com/2013/14/3/R30/abstract) by Philippe et al
        * [Large-scale compression of genomic sequence databases with the Burrows–Wheeler transform](http://bioinformatics.oxfordjournals.org/content/28/11/1415.short) by Cox et al
        * [GPU-Accelerated BWT Construction for Large Collection of Short Reads](http://arxiv.org/pdf/1401.7457v1.pdf) by Liu, Luo, Lam
        * [ropeBWT2](https://github.com/lh3/ropebwt2) by Li (no paper, just a GitHub repo with a README)

* Compression
    * CRAM: [Efficient storage of high throughput DNA sequencing data using reference-based compression](http://genome.cshlp.org/content/21/5/734.long) by Hsi-Yang Fritz et al
    * Quip: [Compression of next-generation sequencing reads aided by highly efficient de novo assembly](http://nar.oxfordjournals.org/content/40/22/e171.short) by Jones et al
    * [Adaptive reference-free compression of sequence quality scores](http://arxiv.org/abs/1305.0159) by Janin, Rosone, Cox
    * [SCALCE: boosting sequence compression algorithms using locally consistent encoding](http://bioinformatics.oxfordjournals.org/content/28/23/3051.full.pdf+html) by Hach et al
    * [Compression of FASTQ and SAM Format Sequencing Data](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0059190) by Bonfield, Mahoney
    * [QualComp: a new lossy compressor for quality scores based on rate distortion theory](http://www.biomedcentral.com/1471-2105/14/187) by Ochoa et al

* Sketching and streaming
    * Background
        * Streaming, Sketching and Sufficient Statistics [part 1](http://www.youtube.com/watch?v=-QSkMcPmXN8), [part 2](http://www.youtube.com/watch?v=twdbZI0lk94) by Cormode
    * eXpress: [Streaming fragment assembly for real-time analysis of sequencing experiments](http://www.nature.com/nmeth/journal/v10/n1/full/nmeth.2251.html) by Roberts, Pachter (also listed above)
    * [Similarity Estimation Techniques from Rounding Algorithms](http://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&ved=0CDAQFjAA&url=http%3A%2F%2Fwww.cs.princeton.edu%2Fcourses%2Farchive%2Fspring04%2Fcos598B%2Fbib%2FCharikarEstim.pdf&ei=BOfGUsqtEbawsASgyYCADg&usg=AFQjCNGhjQeAdc2rz3unSSih-ipPDVDZtw&bvm=bv.58187178,d.cWc) by Charikar
    * [A random-permutations-based approach to fast read alignment](http://www.biomedcentral.com/content/pdf/1471-2105-14-S5-S8.pdf?www.nature.com/doifinder/10.1038/ng.437) by Lederman
    * [Efficient counting of k-mers in DNA sequences using a bloom filter](http://www.biomedcentral.com/1471-2105/12/333) by Melsted, Pritchard
    * [DSK: k-mer counting with very low memory usage](http://bioinformatics.oxfordjournals.org/content/29/5/652.short) by Rizk, Lavenier, Chikhi
    * [Oculus: faster sequence alignment by streaming read compression](http://www.biomedcentral.com/1471-2105/13/297) by Veeneman, Iyer, Chinnaiyan
    * [These are not the k-mers you are looking for: efficient online k-mer counting using a probabilistic data structure](http://arxiv.org/abs/1309.2975) by Zhang et al

* Scalable computing

    * Scalable alignment
        * [CloudBurst: highly sensitive read mapping with MapReduce](http://bioinformatics.oxfordjournals.org/content/25/11/1363.short) by Schatz

    * Scalable indexing
        * [Rapid Parallel Genome Indexing with MapReduce](http://dl.acm.org/citation.cfm?id=1996104) by Menon, Bhat, Schatz
        * [Scalable Parallel Suffix Array Construction](http://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&ved=0CC4QFjAA&url=http%3A%2F%2Falgo2.iti.kit.edu%2Fsanders%2Fpapers%2FKulSan06a.pdf&ei=AfTGUomiDM6-sQSrpoLIDQ&usg=AFQjCNE6pBfaT2JdMwFmycNK4Xg7fs920A&bvm=bv.58187178,d.cWc) by Kulla and Sanders
        * [Parallel Suffix Sorting based on Bucket Pointer Refinement](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=5716066&tag=1) by Mohamed and Abouelhoda

    * Other scalable tools
        * [Searching for SNPs with cloud computing](http://genomebiology.com/2009/10/11/R134) by Langmead et al
        * [Cloud-scale RNA-sequencing differential expression analysis with Myrna](http://genomebiology.com/2010/11/8/R83) by Langmead, Hansen, Leek
        * [ADAM: Genomics Formats and Processing Patterns for Cloud Scale Computing](http://www.eecs.berkeley.edu/Pubs/TechRpts/2013/EECS-2013-207.html) by Massie et al
        * [Fragment assignment in the cloud with eXpress-D](http://www.biomedcentral.com/1471-2105/14/358/abstract) by Roberts, Feng, Pachter (also listed above)
        * [WiggleTools: parallel processing of large collections of genome-wide datasets for visualization and statistical analysis](http://bioinformatics.oxfordjournals.org/content/early/2014/01/07/bioinformatics.btt737.full.pdf) by Zerbino et al
   
Project resources
-----------------

See the [EN 600.439/639](https://github.com/BenLangmead/comp-genomics-class) page for many resources relevant to your final project, including:

* iPython [notebooks describing genomics file formats](https://github.com/BenLangmead/comp-genomics-class/blob/master/README.md#file-format-notebooks) and how to parse them in Python
* iPython [notebooks demonstrating algorithms and data structures](https://github.com/BenLangmead/comp-genomics-class/blob/master/README.md#concept-notebooks) used in genomics
* [Other resources for that class](https://github.com/BenLangmead/comp-genomics-class/blob/master/README.md#file-format-notebooks), including readings, videos, review materials

I've also started to post some [relevant lecture notes](http://www.langmead-lab.org/teaching-materials/) on my lab website.
