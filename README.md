# Automatic Back Transliteration of Romanized Bengali to Bengali (Banglish to Bangla)
 
 Back transliteration of Romanized Bengali to Bengali is the process of converting text written in the Latin alphabet 
 back into the Bengali script. This is often done in order to improve the readability of Bengali text for Bengali speakers 
 by using a simple rules-based system, or an interactive transliteration tool. There are many ways to back transliterate 
 from Romanized Bengali to Bengali, but most of them are either grapheme or phoneme based. This paper introduces a unique 
 pipeline that uses nine open source back transliteration tools to automatically back transliterate Romanized Bengali to 
 Bengali. 
 
 The pipeline consists of seven steps:<br/>
 (1) processing the Romanized Bengali input; <br/> 
 (2) acquiring human transliteration for performance comparison; <br/> 
 (3) employing transliteration tools; <br/> 
 (4) generating candidate transliterations; <br/> 
 (5) post-processing the candidate transliterations; <br/>
 (6) selecting best candidate transliteration, and <br/> 
 (7) evaluating the quality of the transliterations through several performance metrics. 
 
 Experimental results reveal that our approach produced the highest 
 BLEU-1 score of 81.28, BLEU-2 score of 60.75, BLEU-3 score of 44.45, BLEU-4 score of 30.46, and the lowest average word error 
 rate and Word Information Lost of 29.21 and 43.68 respectively on 1000 Romanized Bengali texts. In terms of recall, we 
 achieved a Rouge-L score of 0.7190.

# Repository Structure

There are two folders: Dataset and Codes
+ Dataset: The folder has two excel files. 
	- "1K data Reported in Paper.xlsx" contains 1000 data for reporting the results in the paper.
	- "5K human annotated Banglish to Bangla.xlsx" contains 5000 Banglish sentences along with corresponding human annotated Bengali
+ Codes: Some of the relevant codes.
	- "bnbphoneticparser.py" contains the code for Banglish to Bangla phonetic parser.
	- "gpt.py" contains the code for prompting gpt-3
	- "google_translate_selenium.py" contains the code for translating Banglish sentences to Bangla using selenium.
	- "perplexity.py" contains the code for measuring text quality.
	- To use pyavrophonetic, please refer to https://github.com/auvipy/pyAvroPhonetic
	- To use bntranslit, please refer to https://github.com/sagorbrur/bntranslit
	- To use indic transliteration, please refer to https://github.com/indic-transliteration/indic_transliteration_py
	- To use google transliteration IME, please refer to https://www.google.com/inputtools/try/

# Paper

Accepted version is available at - https://shahariar-shibli.github.io/files/IRAN2022/Banglish_to_Bangla.pdf <br/>
Published version is available at - https://link.springer.com/article/10.1007/s42044-022-00122-9

# Citation
```yaml
@article{shibli2022automatic,
  title={Automatic back transliteration of Romanized Bengali (Banglish) to Bengali},
  author={Shibli, GM Shahariar and Shawon, Md Tanvir Rouf and Nibir, Anik Hassan and Miandad, Md Zabed and Mandal, Nibir Chandra},
  journal={Iran Journal of Computer Science},
  pages={1--12},
  year={2022},
  publisher={Springer}
}
```