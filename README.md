# Large-Obscenity-Lexicon
2000-word list of English-language swear words and other obscenities, including misspellings. Sorted by CommonCrawl rank frequency.

# Creation method

The list is sourced from: manual identification of problem words and morphemes within: 1) the top 5000 most commonly used words appearing in the Common Crawl-trained FastText generic word embeddings; 2) the 5000 words in the FastText Common Crawl embeddings that have the largest frequency rank gap with words appearing in GloVe Wikipedia + Gigaword vector representations. Additional words are searched in the (FastText) vocabulary using the morphemes, and irrelevant hits manually removed.

# Additional variables

Rank reflects frequency rank in the FastText vocabulary. Words can be re-tagged as 'mild' obscenity (swear words, insults, rude language, etc) or not as needed. The last variable reflects whether the words pass a spell check in either US or UK English, per the Hunspell package in R.

# Example

From Preda's 'Wall Street Bets' dataset, see (regularly) flagged words highlighted in red and 'mild' flagged words in orange.

![Reddit Wall Street Bets forum, Example 1](https://github.com/catmoez/Large-Obscenity-Lexicon/blob/main/wsb_titles_censored1.png?raw=true)

![Reddit Wall Street Bets forum, Example 2](https://github.com/catmoez/Large-Obscenity-Lexicon/blob/main/wsb_titles_censored2.png?raw=true)

# Uses

You may wish to detect problematic posts, or words in other forums of text. You can also directly measure which users, speakers, etc. swear at higher rates than others. The lists may also be helpful when creating textual analysis tools, to ensure that you are not including obcene words in various models, lists, etc. that you are releasing, if you do not want them to be kept.

Please feel free to remove words as needed (e.g., in your documents they are used in a formal or legal sense) or to add words as needed. (There are not many disability-related slurs in the current list, for example). 

Please be warned of racial slurs, misogynistic language, etc. in the contents.

# Credit

Credit to: Moez, Catherine. 2024. Large Obscenity Lexicon. (v1, released 23 December 2024). https://github.com/catmoez/Large-Obscenity-Lexicon/.

Many thanks to the Centre for the Politics of Feelings for supporting my research.
