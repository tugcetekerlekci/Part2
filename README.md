# Part2
What is my approach? Why I used it? 
I did linear search while searching the word in the sentences. The reason of that Linear search is good for small lists of unordered elements and it is easy to implement and reasonably efficient. I thought it is simpler approach, simple and less code. I already stored my words and my sentences in an ArrayList at the first part of the project. With this classification, I easily search the words in NER.txt file at the nlp_data.txt file with two nested for loops. 
What are the limitations of my approach? 
My complexity is O(N2) which is not much efficient for huge lists. However the speed is reasonably efficient for the given text files. 
What other approaches might be possible? 
Firstly I thought that hashmap for NER.txt words can be a good way using key-value pairs and look up table. Because, retrieving the known key’s value is fast.I was thought I can use TreeMap because keys will be in natural order. (A,B,C…Z)
With that way I could order the elements with alphabetic order. However it was not also efficient because I will store Archiduke Franz Ferdinand in “A” letter. 
While NER.txt asks Franz Ferdinand the program never find it. 
After that I thought may be I can search all list after controlling specific letter which was a quietly bad idea. Because whether retrieving the known key’s value is fast,  iterating over map is slow. In addition to that, I would use hashCode and equals because I will use my own objects. So I decided to not to move forward with map.
Neither the sentence array and nor word array is sorted to make binary search. Making sort is easy however making list sorted does not benefit to algorithm.

