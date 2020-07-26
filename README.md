# Kannada-Spell-Checker
Spell checker in Kannada

The Kannada context and spelling checker is based on a Trie data structure that is basically a tree kind of structure to store the Kannada words against which the entered text is verified. The Trie data structure stores the common prefixes only once, hence eliminating the extra storage of the words separately like in dictionaries. Also it is efficient and quicker to search the word in the tree rather than searching an entire structure as incase of other data structures such as list. The Kannada words are stored in the form of Unicode and necessary encodings are done wherever required.
If a word on search is present in the Trie then the word is correct otherwise it is considered wrong or displayed as not present. In case the word is wrong then Levenshtein distance is calculated. All the words with one Unicode distance are displayed as suggestions so that the user can select the required word. In case the user wants to add words to the Trie then he/she is free to do so. But this involves shortcomings of adding wrong words to the Trie. To overcome this there has to be a periodic check of the Trie.

