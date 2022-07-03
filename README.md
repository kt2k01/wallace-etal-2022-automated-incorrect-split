# Automated Crossword Solving (Incorrect Split)

Here, I try to see if the word splitter in the ACL 2022 paper [Automated Crossword Solving](https://aclanthology.org/2022.acl-long.219/) work as expected. My intuition is that incorrect splits will have 0 ngram frequency in the Google Books corpus. In the notebook, I use the Google Books ngram API to get the frequencies for the 5-grams. The preliminary results show that the word splitter fail on splitting common words. However, in the paper, it has been implied that the difficulty mainly come from rare words. The results on shorter ngrams need to be further tested. While the longest ngram in the training set is 7-gram, 5-gram is the longest allowed by the API.

Though also shown in the notebook, here are some examples of incorrect split:
- your ownside of the bed
- they do when i hitthesack
- ounce in a blue moon
- to stayinan area of a
- otidings of comfort and joy