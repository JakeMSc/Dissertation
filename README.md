## Amplifi Dissertation

### Abstract

Over 90% of consumers sign terms and conditions without reading them.  Major reasons for this include excessive word lengths and the use of legal language incomprehensible to non-legal experts. The consequences of this in the finance sector are severe.  Consumers apply for financial products they do not understand.  Some banks exploit this vulnerability, leading to major scandals that have cost UK retail banks over £72 billion in misconduct expenses since 2000. The Financial Conduct Authority expects the number of vulnerable consumers to rise in the fallout of the COVID-19 Pandemic.  To mitigate this,  this project aims to create an automated terms and conditions summarisation and language simplification system in a bid to increase comprehension and consumer engagement with terms and conditions. Utilising transformer models pre-trained on large corpora and fine-tuned on a task of summarising terms and conditions clauses, we were able to compress terms and conditions to 20% of their original length, and reduce the level of education required for comprehension from post-graduate levels down to high-school levels.

### Files

Terms_Scraping.ipynb contains a script for scraping terms and conditions from a list of website URLs.

Pegasus_Masking.ipynb contains a script for preparing documents for the gap-sentence generation pre-training task of Pegasus.

Pegasus_training_data_medium.csv contains terms and conditions scraped by Terms_scraping.ipynb and prepared by Pegasus_Masking.ipynb.

Pretraining_Pegasus contains a script for domain-adaptive pre-training of Pegasus using data prepared by Pegasus_masking.ipynb.

Fine_Tuning.ipynb contains a script for fine-tuning transformers for abstractive summarisation with HuggingFace.
