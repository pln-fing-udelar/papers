### QA Intro
- Martin & Jurafsky, 3era ed. Capítulo 23: Question Answering [Link](https://web.stanford.edu/~jurafsky/slp3/23.pdf)


### Papers sobre Information Retrieval en el marco de QA

- Moldovan, D., & Surdeanu, M. (2002, July). On the role of information retrieval and information extraction in question answering systems. 
In _International Summer School on Information Extraction_ (pp. 129-147). Springer, Berlin, Heidelberg. [Link](https://link.springer.com/chapter/10.1007/978-3-540-45092-4_6)

- Libro de IR: Manning, C. D., Raghavan, P., and Schu ̈tze, H. (2008). In- troduction to Information Retrieval. Cambridge.[Link](https://nlp.stanford.edu/IR-book/pdf/irbookonlinereading.pdf)

- Karpukhin, V., Og ̆uz, B., Min, S., Lewis, P., Wu, L., Edunov, S., Chen, D., and Yih, W.-t. (2020). Dense passage retrieval for open-domain question answering. EMNLP. [Link](https://arxiv.org/pdf/2004.04906.pdf)

Abstract
Open-domain question answering relies on ef- ficient passage retrieval to select candidate contexts, where traditional sparse vector space models, such as TF-IDF or BM25, are the de facto method. In this work, we show that retrieval can be practically implemented us- ing dense representations alone, where em- beddings are learned from a small number of questions and passages by a simple dual- encoder framework. When evaluated on a wide range of open-domain QA datasets, our dense retriever outperforms a strong Lucene- BM25 system greatly by 9%-19% absolute in terms of top-20 passage retrieval accuracy, and helps our end-to-end QA system establish new state-of-the-art on multiple open-domain QA benchmarks.1

- Chen, D., Fisch, A., Weston, J., and Bordes, A. (2017). Reading wikipedia to answer open-domain questions. ACL. [Link](https://arxiv.org/pdf/1704.00051.pdf)

Abstract
This paper proposes to tackle open- domain question answering using Wikipedia as the unique knowledge source: the answer to any factoid question is a text span in a Wikipedia article. This task of machine reading at scale combines the challenges of document re- trieval (finding the relevant articles) with that of machine comprehension of text (identifying the answer spans from those articles). Our approach combines a search component based on bigram hashing and TF-IDF matching with a multi-layer recurrent neural network model trained to detect answers in Wikipedia paragraphs. Our experiments on multiple existing QA datasets indicate that (1) both modules are highly competitive with respect to existing counterparts and (2) multitask learning using distant supervision on their combination is an effective complete system on this challenging task.


- Lin, J., Nogueira, R., and Yates, A. (2020). Pretrained transformers for text ranking: BERT and beyond. arXiv preprint arXiv:2010.06467. [Link](https://arxiv.org/pdf/2010.06467.pdf) 

Abstract
The goal of text ranking is to generate an ordered list of texts retrieved from a corpus in response to a query for a particular task. Although the most common formulation of text ranking is search, instances of the task can also be found in many natural language processing applications. This survey provides an overview of text ranking with neural network architectures known as transformers, of which BERT is the best-known example. The combination of transformers and self-supervised pretraining has, without exaggeration, revolutionized the fields of natural language processing (NLP), information retrieval (IR), and beyond. In the context of text ranking, these models produce high quality results across many domains, tasks, and settings.
In this survey, we provide a synthesis of existing work as a single point of entry for practitioners who wish to gain a better understanding of how to apply transformers to text ranking problems and researchers who wish to pursue work in this area. We cover a wide range of modern techniques, grouped into two high-level categories: transformer models that perform reranking in multi-stage ranking architectures and learned dense representations that attempt to perform ranking directly. There are numerous examples that fall into the first category, including approaches based on relevance classification, evidence aggregation from multiple segments of text, corpus analysis, and sequence-to-sequence models. While the second category of approaches is less well studied, representation learning with transformers is an emerging and exciting direction that is bound to attract more attention moving forward. There are two themes that pervade our survey: techniques for handling long documents, beyond the typical sentence-by-sentence processing approaches used in NLP, and techniques for addressing the tradeoff between effectiveness (result quality) and efficiency (query latency).
Although transformer architectures and pretraining techniques are recent innova- tions, many aspects of how they are applied to text ranking are relatively well understood and represent mature techniques. However, there remain many open research questions, and thus in addition to laying out the foundations of pretrained transformers for text ranking, this survey also attempts to prognosticate where the field is heading.

- Kamphuis, C., de Vries, A. P., Boytsov, L., and Lin, J. (2020). Which bm25 do you mean? a large-scale repro- ducibility study of scoring variants. European Conference on Information Retrieval. [Link](https://link.springer.com/chapter/10.1007/978-3-030-45442-5_4) 

Abstract
When researchers speak of BM25, it is not entirely clear which variant they mean, since many tweaks to Robertson et al.’s original formulation have been proposed. When practitioners speak of BM25, they most likely refer to the implementation in the Lucene open-source search library. Does this ambiguity “matter”? We attempt to answer this question with a large-scale reproducibility study of BM25, considering eight variants. Experiments on three newswire collections show that there are no significant effectiveness differences between them, including Lucene’s often maligned approximation of document length. As an added benefit, our empirical approach takes advantage of databases for rapid IR prototyping, which validates both the feasibility and methodological advantages claimed in previous work.
