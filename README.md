# HashMap_Linearprobing
Implement HashMap Linear Probing in Python3


# Whats Linear probing ?
In linear probing technique, collision is resolved by searching linearly in the hash table until an empty location is found. Its also called "Open Addressing Technique".
The search for open slot starts from the slot where the collision happened. It moves sequentially through the slots until an empty slot is encountered. The movement is in a circular fashion. It can move to the first slot while searching for an empty slot. Hence, covering the entire hash table. 

All the elements are stored in HashMap itself and at any point of time, size of the table must be greater than the total number of keys.

Insert(k): Keep probing until an empty slot is found. Once an empty slot is found, insert k. 

Search(k): Keep probing until slot’s key doesn’t become equal to k or an empty slot is reached. 

Delete(k): If we simply delete a key, then the search may fail. So slots of deleted keys are marked specially as “deleted”. 
The insert can insert an item in a deleted slot, but the search doesn’t stop at a deleted slot. 

Good resource : https://www.cs.tau.ac.il/~zwick/Adv-Alg-2015/Linear-Probing.pdf
