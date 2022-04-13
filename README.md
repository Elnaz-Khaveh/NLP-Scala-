# NLP-Scala-
The project done in NLP on wikipedia articles by Scala


(a) Extracts (i) words (i.e., sequences of the
letters “a-z” including dashes “-” and under-dashes “ ”) and (ii) numbers (i.e., sequences of the
digits “0-9” separated by at most one “.”) into two separate RDD objects. 

(b) For the set of 41,784 Wikipedia articles
provided on Moodle in order to find the (i) top-1,000 most frequent words and the (ii) top-1,000 most
frequent numbers contained among all articles, respectively. Sort the words and numbers from the
two RDDs in descending order of their counts, and finally store the two lists of sorted numbers and
words in two separate files on your local file system. Compare the results with the ones you obtained
via Hadoop in Problem 1 and explain possible differences in your Problem 2.txt file.

(c) Parse the file stopwords.txt into a sequence object (i.e., an Array or a List)
such that each stopword becomes one entry in this sequence, and store the sequence as an immutable
variable val stopwords = ... in your Spark environment. Refer to the modified parsing function
for words you implemented in (a) and filter out all stopwords from the RDD holding the words
by referring to val stopwords in the closure of your filtering function. Finally, compute the word
counts of the remaining words as before.  

(d) Repeat the steps of (c) but this time create a new broadcast variable in your Spark environment
to store the stopwords. Compute the word counts of the filtered words as before and compare the
runtime of this approach to the one of (c).
