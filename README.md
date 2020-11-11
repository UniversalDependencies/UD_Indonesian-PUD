# Summary

This is a part of the Parallel Universal Dependencies (PUD) treebanks created
for the [CoNLL 2017 shared task on Multilingual Parsing from Raw Text to
Universal Dependencies](http://universaldependencies.org/conll17/).


# Introduction

There are 1000 sentences in each language, always in the same order. (The sentence
alignment is 1-1 but occasionally a sentence-level segment actually consists
of two real sentences.) The sentences are taken from the news domain (sentence
id starts in ‘n’) and from Wikipedia (sentence id starts with ‘w’). There are
usually only a few sentences from each document, selected randomly, not
necessarily adjacent. The digits on the second and third position in the
sentence ids encode the original language of the sentence. The first 750
sentences are originally English (01). The remaining 250 sentences are
originally German (02), French (03), Italian (04) or Spanish (05) and they
were translated to other languages via English. Translation into German,
French, Italian, Spanish, Arabic, Hindi, Chinese, Indonesian, Japanese,
Korean, Portuguese, Russian, Thai and Turkish has been provided by DFKI and
performed (except for German) by professional translators. Then the data has
been annotated morphologically and syntactically by Google according to Google
universal annotation guidelines; finally, it has been converted by members of
the UD community to UD v2 guidelines.

Additional languages have been provided (both translation and native UD v2
annotation) by other teams: Czech by Charles University, Finnish by University
of Turku and Swedish by Uppsala University.

The entire treebank is labeled as test set (and was used for testing in the
shared task). If it is used for training in future research, the users should
employ ten-fold cross-validation.

==================
README FROM UI
==================

A reseach team from Faculty of Computer Science, Universitas Indonesia (UI) proposed a revision to Indonesian PUD in 2019 and 2020.

A description of how the Indonesian PUD was manually revised by UI  can be found in Alfina et al. (2019) and Alfina et al. (2020) in the references section. The short description about the annotation guidelines can be found in [Indonesian Documentation](https://universaldependencies.org/id/index.html).

The original repository of the revised Indonesian PUD conducted by UI can be found [here](https://github.com/ialfina/revised-id-pud).

==================
README FROM GOOGLE
==================

A description of how the treebanks were generated can be found in:

  Universal Dependency Annotation for Multilingual Parsing
  Ryan McDonald, Joakim Nivre, Yvonne Quirmbach-Brundage, Yoav Goldberg,
  Dipanjan Das, Kuzman Ganchev, Keith Hall, Slav Petrov, Hao Zhang,
  Oscar Tackstrom, Claudia Bedini, Nuria Bertomeu Castello and Jungmee Lee
  Proceedings of ACL 2013

A more detailed description of each relation type in our harmonized scheme is
included in the file universal-guidelines.pdf.

Each file is formatted according to the CoNLL 2006/2007 guidelines:

  http://ilk.uvt.nl/conll/#dataformat

The treebank annotations use basic Stanford Style dependencies, modified
minimally to be sufficient for each language and be maximally consistent across
languages. The original English Stanford guidelines can be found here:

  http://nlp.stanford.edu/software/dependencies_manual.pdf

================================
Fine-grained part-of-speech tags
================================

In the CoNLL file format there is a coarse part-of-speech tag field (4) and a
fine-grained part-of-speech tag field (5). In this data release, we use the
coarse field to store the normalized universal part-of-speech tags that are
consistent across languages. The fine-grained field contains potentially richer
part-of-speech information depending on the language, e.g., a richer tag
representation for clitics.

=========================
Licenses and terms-of-use
=========================

We will distinguish between two portions of the data:

1. The underlying text for sentences and corresponding translations. This data Google asserts no ownership over and no copyright over. The source of the texts is randomly selected Wikipedia (www.wikipedia.org) sentences. Some or all of these sentences may be copyrighted in some jurisdictions. Where copyrighted, Google collected these sentences under exceptions to copyright or implied license rights.  GOOGLE MAKES THEM AVAILABLE TO YOU under CC-BY-SA 3.0, WITHOUT ANY WARRANTY OF ANY KIND, WHETHER EXPRESS OR IMPLIED.See attached LICENSE file for the text of CC BY-SA 3.0.

2. The annotations -- part-of-speech tags and dependency annotations. GOOGLE MAKES THEM AVAILABLE TO YOU 'AS IS', WITHOUT ANY WARRANTY OF ANY KIND, WHETHER EXPRESS OR IMPLIED.


# Acknowledgments

## From Google:
We are greatful to the many people who made this dataset possible:
Fernando Pereira, Hans Uszkoreit, Aljoscha Burchardt, Vivien Macketanz,
Ali Elkahky, Abhijit Barde, Tolga Kayadelen, ...

## From UI:
We thank the contributors of the revision project of the Indonesian PUD:
* Designers of the Indonesian annotation guidelines: Ika Alfina, Daniel Zeman, Arawinda Dinakaramani
* Annotators: Ika Alfina, Arawinda Dinakaramani, Muhammad Yudistira Hanifmuti, Jessica Naraiswari Arwidarasti, Yogi Lesmana Sulestio

## References
* Ika Alfina, Daniel Zeman, Arawinda Dinakaramani, Indra Budi, and Heru Suhartanto. "**Selecting the UD v2 Morphological Features for Indonesian Dependency Treebank**". In Proceedings of the 2020 International Conference of Asian Language Processing (IALP)  in Kuala Lumpur, Malaysia, 4-6 Desember 2020. (_accepted_)
* Ika Alfina, Arawinda Dinakaramani, Mohamad Ivan Fanany, and Heru Suhartanto. ["**A Gold Standard Dependency Treebank for Indonesian**"](https://waseda.repo.nii.ac.jp/?action=repository_action_common_download&item_id=48059&item_no=1&attribute_id=101&file_no=1). In Proceedings of 33rd Pacific Asia Conference on Language, Information and Computation (PACLIC) 2019 in Hakodate, Japan, 13-15 September 2019. 
* Ryan McDonald, Joakim Nivre, Yvonne Quirmbach-Brundage, Yoav Goldberg, Dipanjan Das, Kuzman Ganchev, Keith Hall, Slav Petrov, Hao Zhang, Oscar Tackstrom, Claudia Bedini, Nuria Bertomeu Castello and Jungmee Lee. "**Universal Dependency Annotation for Multilingual Parsing**". In Proceedings of ACL 2013.


# Changelog
* 2020-11-15 v2.7
  * Manual revision conducted by Alfina et al. from Universitas Indonesia. They conducted major revision on word segmentation, POS tagging, morphological features, and syntactic annotation.
* 2018-07-01 v2.2
  * First official release after it was used as a surprise dataset in the
    CoNLL 2018 shared task.

=======
Contact
=======

slav@google.com
ika.alfina@cs.ui.ac.id

=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.2
License: CC BY-SA 3.0
Includes text: yes
Genre: news wiki
Lemmas: manual native
UPOS: manual native
XPOS: not available
Features: manual native
Relations: manual native
Contributors: Uszkoreit, Hans; Macketanz, Vivien; Burchardt, Aljoscha; Harris, Kim; Marheinecke, Katrin; Petrov, Slav; Kayadelen, Tolga; Attia, Mohammed; Elkahky, Ali; Yu, Zhuoran; Pitler, Emily; Lertpradit, Saran; Manurung, Ruli; Shohibussirri, Muh; Popel, Martin; Zeman, Daniel; Alfina, Ika; Dinakaramani, Arawinda; Hanifmuti, Muhammad Yudistira; Arwidarasti, Jessica Naraiswari; Sulestio, Yogi Lesmana
Contributing: here
Contact: ika.alfina@cs.ui.ac.id
===============================================================================
