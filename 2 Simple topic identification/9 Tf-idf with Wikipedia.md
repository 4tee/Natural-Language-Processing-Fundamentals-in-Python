# Tf-idf with Wikipedia #

Now it's your turn to determine new significant terms for your corpus by applying `gensim`'s tf-idf. You will again have access to the same corpus and dictionary objects you created in the previous exercises - `dictionary`, `corpus`, and `doc`. Will tf-idf make for more interesting results on the document level?

## Instructions ##

* Import `TfidfModel` from `gensim.models.tfidfmodel`.
* Initialize a new `TfidfModel` called `tfidf` using `corpus`.
* Use `doc` to calculate the weights. You can do this by passing `[doc]` to `tfidf`.
* Print the first five term ids with weights.
* Sort the term ids and weights in a new list from highest to lowest weight. This has been done for you.
* Print the top five weighted words (`term_id`) from `sorted_tfidf_weights` along with their weighted score (`weight`).

```python
# Import TfidfModel
from gensim.models.tfidfmodel import TfidfModel

# Create a new TfidfModel using the corpus: tfidf
tfidf = TfidfModel(corpus)

# Calculate the tfidf weights of doc: tfidf_weights
tfidf_weights = tfidf[doc]

# Print the first five weights
print(tfidf_weights[:5])

# Sort the weights from highest to lowest: sorted_tfidf_weights
sorted_tfidf_weights = sorted(tfidf_weights, key=lambda w: w[1], reverse=True)

# Print the top 5 weighted words
for term_id, weight in sorted_tfidf_weights[:5]:
    print(dictionary[term_id], weight)
```

```
[(24, 0.0022836332291091273), (39, 0.0043409401554717324), (41, 0.008681880310943465), (55, 0.011988285029371418), (56, 0.005482756770026296)]
reverse 0.4884961428651127
infringement 0.18674529210288995
engineering 0.16395041814479536
interoperability 0.12449686140192663
reverse-engineered 0.12449686140192663
```