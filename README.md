# Automatic Back Transliteration of Romanized Bengali to Bengali
 
 Back transliteration of Romanized Bengali to Bengali is the process of converting text written in the Latin alphabet 
 back into the Bengali script. This is often done in order to improve the readability of Bengali text for Bengali speakers 
 by using a simple rules-based system, or an interactive transliteration tool. There are many ways to back transliterate 
 from Romanized Bengali to Bengali, but most of them are either grapheme or phoneme based. This paper introduces a unique 
 pipeline that uses nine open source back transliteration tools to automatically back transliterate Romanized Bengali to 
 Bengali. The pipeline consists of seven steps: (1) processing the Romanized Bengali input; (2) acquiring human transliteration 
 for performance comparison; (3) employing transliteration tools; (4) generating candidate transliterations; (5) post-processing 
 the candidate transliterations; (6) selecting best candidate transliteration, and (7) evaluating the quality of the 
 transliterations through several performance metrics. Experimental results reveal that our approach produced the highest 
 BLEU-1 score of 81.28, BLEU-2 score of 60.75, BLEU-3 score of 44.45, BLEU-4 score of 30.46, and the lowest average word error 
 rate and Word Information Lost of 29.21 and 43.68 respectively on 1000 Romanized Bengali texts. In terms of recall, we 
 achieved a Rouge-L score of 0.7190.
