### Tree
#### Trie

It's a tree data structure for storing strings. It can search if a string exists in the collection in O(m) time where m is length of the string. It facilitates prefix search and can sort the string in lexicographical order.   

Each node contains a map <Character, TrieNode> and Boolean stringEnded. Insertion of a string into trie iterate through character in string and put charater into individual trie nodes starting at root. If current node map doesn't have the character , new entry<Character, TrieNode> will be created and acts as a pointer from current node to next.  

HashMap can store string and allow O(1) if exist operation but doesn't has feature of lexical sort and prefix search that present in Trie.  

