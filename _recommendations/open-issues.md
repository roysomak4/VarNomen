---
layout: default-md
title: Open Issues
order: 6
---

# {{page.title}}

* * *

## Community Consultation

There are currently no proposals open for [_Community Consultation_](/bg-material/consultation/). Proposal [_SVD-WG004 (ISCN<>HGVS)_](/bg-material/consultation/svd-wg004/) to extend the recommendations to cover the description of structural variants, esp. translocations and chromothripsis closed Jan.15 (2016) and is currently _under review_. Proposal {{site.baseurl}}[_SVD-WG003 (exon del/dup)_](/bg-material/consultation/svd-wg003/) with the suggesting to describe exon deletions/duplications using the format c.(233+1\_234-1)\_(1234+1\_1235-1)del, closed Jul.16 (2015), is prepared for a new round of consultation.


* * *

<a name ="opentopics"></a>

## Open topics

<a name ="geneflanking"></a>

### Numbering gene flanking nucleotides

The current recommendation to describe variants based on a coding DNA reference sequence is to use "c.-" numbers for nucleotides 5' of the ATG translation initiation codon and "c.\*" numbers for nucleotides 53' of the translation termination codon [_see Numbering_](/bg-material/numbering/). However, such descriptions do not show whether the nucleotides are **inside or outside** the transcribed region. The request has been filed (_PEM Taschner, Leiden, Nederland_) to make a discrimination between transcribed and un-transcribed nucleotides using the format;

*	c.-N-uM  =  nucleotide uM is at position -M upstream (u) of nucleotide c.-N, the transcription initiation site of the reference transcript, e.g. c.-237-u29A>G (currently c.266A>G)
	:	_**NOTE**_:	restricted to nucleotides 5' of the transcription initiation site (cap site), i.e. upstream of the gene (incl. the promoter)
*	c.\*N+dM  =  nucleotide dM is at position +M downstream (d) of nucleotide c.\*N, the polyA-addition site of the reference transcript, e.g. \*237+d133A>G (currently c.\*370A>G)
	:	_**NOTE**_:	restricted to nucleotides 3' of the polyA-addition site, i.e. downstream of the gene

<a name ="imperfectcopy"></a>

### Imperfect copies

HGVS nomenclature has excellent possibilities to describe large duplications, inversions, conversions and insertions. However, no clear recommendations are available what to do when the nucleotides involved are not a perfect copy of the original sequence. The suggestion has been made ([_Taschner PEM, Den Dunnen JT (2011). Hum.Mutat. 32:507-511_](http://onlinelibrary.wiley.com/doi/10.1002/humu.21427/pdf) to use "**{ }**" (curly braces) as a kind of "_sub-alleles_" to describe the variants in the altered region.
*	g.24_65dup{46G>T}
	:	a duplication of nucleotides g.24 to g.65 with variant g.46G>T in the duplicated copy.

<a name ="extensions"></a>

### Protein Extensions

Would you consider a small change in the suggested nomenclature for the [_description of extensions_](/recommendations/protein/variant/extension/) from p.*110Glnext*17 to p.*110Glnext17? (_Yael Shinar, Tel Hashomer, Israel_)

The description of extensions can probably indeed be simplified. While for **extensions** we currently give the position of the new translation initiation (start) codon as "-5" or of the termination (stop) codon as "\*17" this is strictly speaking not necessary. By defenition the extension goes upstream for an N-terminal change and downstream for a C-terminal change. Using p.Met1ext5 (now p.Met1ext-5) and p.\*110Glnext17 (now p.\*110Glnext\*17) therefore seems sufficient.

<a name ="modifications"></a>

### Modifications

Aug.24 (2011) - JT den Dunnen
HGVS nomenclature does currently not have recommendations for the descriptions of modifications of DNA, RNA or protein molecules. The most pressing need for a recommendation is are DNA methylation and RNA editing.

#### RNA editing

Addition of RNA editing data to a DNA variant database seems a sensible thing to do. An RNA-based sequencing study might reveal an interesting variant which, when checked in the database, is listed (...RNA editing data is not recorded). This will trigger a DNA sequencing experiment, trying to confirm the variant, which will fail since the variant is not present at the DNA level and valuable resources are spoiled.

The suggestion is to describe RNA editing using "**@**";

*	g.1287@ (based on a genomic reference sequence)
*	c.143@ (based on a coding DNA reference sequence)
*	n.143@ (based on a non-coding DNA reference sequence)
*	r.143c@u on RNA level (or the observed change r.143c>u)
*	p.(His48Pro) on protein level (i.e. the predicted consequence)

The use of the "**@**" character versus other characters (&, $, ~, #) is of course debatable. Another option is to use a three-letter abbreviation like "del" and "ins", e.g. "**edt**" (g.1287Cedt / c.143Cedt) but this is seems less attractive (longer and potentially confusing). The "**@**" should serve as a simple mark, indicating 'note this site, something is happening at ("**@**") this position.

Using the description r.143c>u on RNA level suggests a substitution. There are several types of RNA editing and "r.143c" probably does not really change to a "u". All we can say is that the polymerases used to make a copy inserted an "a". At some point we probably need to suggest ways to exactly describe the chemical modification made by the RNA editing enzyme but we can do that later. Making such recommendations can then be combined with those for DNA modifications (like methylation with methyl or hydroxy-methyl groups) making sure they follow the same rules.

The question is whether we need a specific description at the DNA level indicating that the nucleotide is known to be modified at RNA level. The main purpose of this mark would be to facilitate easy database retrieval of such sites. Approval of proposal [_SVD-WG001_](http://www.hgvs.org/mutnomen/accepted001.html) more or less opened the option for such marks.

<a name ="exonnumbering"></a>

### Exon Numbering

HGVS nomenclature does not give specific recommendations for the **numbering of exons**. For variant descriptions exon numbers are not required, **nucleotide position are sufficient**. In many genes there is no consensus on exon/intron numbering and several old numbering schemes may exist that had to be revised to include newly discovered exons (internal as well as 5' and/or 3' of the gene). This led to all kinds of numbering schemes with no clear structure, making it very difficult for non-experts in the specific gene to keep track of all details (see also [Dalgleish 2010](http://www.genomemedicine.com/content/pdf/gm145.pdf){:target="_blank"} and [NCBI RefSeqGene](http://www.ncbi.nlm.nih.gov/refseq/rsg/faq/#exon){:target="_blank"}). To prevent confusion and with the increasing use of genome browsers, numbering exons simply as 1, 2, 3, etc., from start to the end is the only logical option.
	Although this is probably difficult to accept by the experts, we can not keep on confusing newcomers by forever using legacy numbering systems. We should realize that, at some point, wrong assumptions will be made with as a consequence a patient will receive an erroneous diagnosis. This is of course unacceptable.

*	The CBS gene was originally thought to contain 16 exons. Later it was recognised that exon 15 does not exist, and recently two additional non-translated 5' exons were detected. The current gene structure therefore includes 17 exons, of which exons 3 to 17 are translated. Should the exons of a gene be counted from the exon that contains the start codon rather than the beginning of the cDNA?  If so, should exons preceding the start codon be counted 0, -1, -2, etc. or should the 0 be skipped?  Is there an agreement on how to deal with changes in exon numbering?
	:	For the description of sequence changes it does not matter how exons are numbered,  exon (and intron) numbers are not used in the descriptions, only nucleotide positions. For exon numbering the only logical thing to do is to start with 1 for the first exon and number all following exons successively. Using other numbering schemes problems will emerge at some point. Note that when alternative numbering schemes are used, these will only be recognised by experts in the field knowing their history; newcomers just blindly assume that the first exon annotated in the genome is exon 1. Consequently, when legacy numbering schemes are used, this will cause confusion and at some point wrong assumptions will be made and a patient might end up with an erroneous diagnosis. In papers, when used, specifically mention how exons were numbered (M&M, Figure and Table legends). For tables, consider to add a column listing the historic / old exon numbers.
