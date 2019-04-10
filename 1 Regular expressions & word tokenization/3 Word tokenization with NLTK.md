# Word tokenization with NLTK #

Here, you'll be using the first scene of Monty Python's Holy Grail, which has been pre-loaded as `scene_one`. Feel free to check it out in the IPython Shell!

Your job in this exercise is to utilize `word_tokenize` and `sent_tokenize` from `nltk.tokenize` to tokenize both words and sentences from Python strings - in this case, the first scene of Monty Python's Holy Grail.

## Instructions ##

* Import the `sent_tokenize` and `word_tokenize` functions from `nltk.tokenize`.
* Tokenize all the sentences in `scene_one` using the `sent_tokenize()` function.
* Tokenize the fourth sentence in `sentences`, which you can access as `sentences[3]`, using the `word_tokenize()` function.
* Find the unique tokens in the entire scene by using `word_tokenize()` on `scene_one` and then converting it into a set using `set()`.
* Print the unique tokens found. This has been done for you, so hit 'Submit Answer' to see the results!

```python
# Import necessary modules
from nltk.tokenize import sent_tokenize
from nltk.tokenize import word_tokenize

# Split scene_one into sentences: sentences
sentences = sent_tokenize(scene_one)

# Use word_tokenize to tokenize the fourth sentence: tokenized_sent
tokenized_sent = word_tokenize(sentences[3])

# Make a set of unique tokens in the entire scene: unique_tokens
unique_tokens = set(word_tokenize(scene_one))

# Print the unique tokens result
print(unique_tokens)
```

```
{'Whoa', 'ridden', 'do', 'an', 'ask', 'coconut', 'Court', 'is', 'martin', 'mean', 'why', 'creeper', 'them', 'son', 'together', 'Well', 'maintain', 'held', 'sovereign', 'They', 'the', 'court', '!', 'England', 'this', 'have', 'course', 'minute', 'just', 'climes', 'It', 'strangers', "n't", 'order', 'length', 'not', 'am', ',', 'Pull', 'We', '--', 'our', 'Am', 'or', 'Oh', '.', 'Britons', 'bangin', 'goes', 'A', 'carried', 'times', 'tell', 'my', 'there', 'temperate', 'who', 'south', 'yet', 'does', 'house', 'King', 'So', 'European', 'all', 'he', 'then', 'feathers', 'weight', 'coconuts', 'question', 'But', 'Where', 'Are', 'grip', 'The', 'anyway', 'may', 'servant', 'Uther', 'every', 'swallow', 'Patsy', 'forty-three', 'but', 'me', 'Will', 'African', 'Halt', 'five', 'empty', 'two', 'That', 'Who', 'No', 'needs', '...', 'lord', 'will', 'get', 'kingdom', 'of', 'knights', 'Supposing', 'Mercea', 'go', 'interested', 'must', '1', 'Please', 'fly', 'carrying', 'by', '[', 'velocity', 'wings', 'your', 'Wait', 'In', ':', 'ARTHUR', 'covered', "'ve", 'wants', 'bring', 'line', 'search', 'What', 'beat', 'it', 'found', 'carry', 'got', "'m", 'plover', 'to', 'air-speed', 'husk', 'you', 'Yes', 'wind', '#', 'Pendragon', 'speak', 'are', 'ratios', 'pound', 'in', 'clop', '?', 'if', "'s", 'bird', 'You', 'they', 'through', 'ounce', 'its', 'suggesting', 'here', 'back', 'I', 'could', 'seek', "'re", 'use', 'and', ']', 'SCENE', 'master', 'simple', 'breadth', 'sun', 'horse', 'yeah', 'Saxons', 'guiding', 'tropical', "'em", 'SOLDIER', 'land', 'at', 'dorsal', 'Camelot', 'maybe', "'d", 'with', 'winter', 'Not', 'from', 'warmer', 'Arthur', 'right', 'matter', '2', 'snows', 'Listen', 'agree', 'using', 'under', 'join', 'that', 'be', 'point', 'on', 'non-migratory', 'castle', 'KING', 'halves', 'Found', 'these', 'strand', "'", 'second', 'zone', 'other', 'Ridden', 'defeator', 'migrate', 'where', 'grips', 'trusty', 'a', 'since', 'swallows', 'one'}
```