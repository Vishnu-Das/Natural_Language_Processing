# One Hot Encoding

![alt text](image.png)

Using the vocabulary we assign each word with a bit representation.

**Then each sentence can be represented as an array of these bit representations of words, which result in a matrix of n * m where n = number of words in the sentence and m = number of unique words or voccabularies**

## Advantage
- Easy to implement with python. in sklearn we have one code encoder, also in pandas pd.get_dummies

## Disadvantages
- Sparse matrix : That is lot of ones and zeroes. This leads to **overfitting**
- No Fixed Size of matrix : Depends on the length of the word. mentioned as (n) above.
- No semantic meaning is getting captured. cosin similarity we cant find since all the vectors are equi distant and does not retain relation between vectors
- Will not work when new word comes that is not present in the vocabs