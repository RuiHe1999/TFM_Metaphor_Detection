# General Description
This is a description of the data used in this study. 

**Dataset format**:

All Datasets are endcoded with UTF-8. The datasets we shared here are not original ones but formatted into 5 or 8 columns.

| Column Title            | Meaning                   | Note                                     |
| ------------            | -----------------------   | ---------------------------------------- |
| sent_index              | Sentence Index            |                                          |
| sent_txt                | Original Sentence         |                                          |
| pos_seq                 | POS tag sequence          |                                          |
| metaphor_seq            | metaphor label sequence   | binary, 0 for literal and 1 for metaphor |
| genre                   | source text genre         | news, fiction, academic, conversation (conversation only in VUA) |
| sent_txt_tokenized      | orignial tokenization     |                                          |
| sent_bert_tokens        | bert tokenization         |                                          |
| sent_txt_tokenized_bert | bert tokenization in the style of  original tokenization |           |
| BIO_seq                 | BIO tag sequence          | trinary, B for begining of metaphor, I for inside metaphor and O for outside metaphor (i.e. literal) |
| split                   | subset label              | trinary, train/test/val                  |

## VUA
VUA dataset is an English metaphor dataset obtained from [Shared Task on Metaphor Detection](<https://github.com/EducationalTestingService/metaphor/tree/master/VUA-shared-task>). 

## PSUCMC
The PSU Chinese Metaphor Corpus is published by Dr. Xiaofei Lu on his [personal webset](<http://www.personal.psu.edu/xxl13/downloads/cmc.html>).

There are some errors in the original corpus which we fixed them manually

- fiction\_10\_v.4.txt: 
0013: This is resulted from a blank space which is not recognized by the html parser. As the blank space here is not grammatically suitable in Chinese, I deleted it in the corpus. 

- news\_10\_v.4.txt: 0077 
This is resulted from the omission of > in the original corpus, I added it.

- news\_17\_v.4.txt: 0025 
This is due to a bad format in the original corpus (additional blank line), I changed it.

 - news\_20\_v.4.txt: 0021 
This is due to a lack of </s\> in the original corpus, I added it.