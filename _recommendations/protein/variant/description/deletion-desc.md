---
parent: Protein
title: deletion
category: description
---

Format:  **"prefix""amino_acid(s)+position(s)_deleted""del"**,  e.g. p.Cys76\_Glu79del

**"prefix"**  =  reference sequence used  =  p.<br>
**"amino_acid(s)+position(s)_deleted"**  =  amino acid with position or range (first amino acid with position to last amino acids with position) deleted  =  Cys76\_Glu79<br>
**"del"**  =  type of change is a deletion =  del

---

### Note

*	**prefix** reference sequence accepted is "p." (protein).
*	predicted consequences, i.e. without experimental evidence (no RNA or protein analysed), should be given in parentheses, e.g. p.(Arg727\_Ser783del).
*	the "amino\_acids+positions\_deleted" should contain **two different** positions, e.g. Cys76\_Glu79, not Cys76\_Cys76.
*	the "positions\_deleted" should be listed from **5' to 3'**, e.g. Cys76\_Glu79, not Glu79\_Cys76.
*	for all descriptions the **most C-terminal position** possible of the reference sequence is arbitrarily assigned to have been changed (_**3'rule**_).
	*	the 3'rule also applies for changes in single amino acid stretches and tandem repeats.
*	variants should be described on the protein level and not incorporate knowledge regarding the change at the DNA level.
*   in theory, a **nonsense** variant can be considered as a deletion removing the C-terminal end of the protein (e.g. p.Trp26\_Arg1623del). However, in HGVS nomenclature, nonsense variants are described as an amino acid substitution (p.Trp26Ter or p.Trp26* [_see Substitution_](/recommendations/protein/variant/substitution)) replacing the first amino acid affected by a translation termination (stop) codon.
