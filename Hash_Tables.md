# Hash Tables

## WHY - The Importance of Hash Tables:

Hash tables are fundamental data structures in computer science with various applications. Here's why they are important:

1. Fast Data Retrieval: Hash tables provide fast and efficient data retrieval. They enable constant-time (O(1)) access to values based on their keys, making them incredibly efficient for tasks like searching and indexing.

2. Data Organization: Hash tables help organize and manage large datasets. They allow you to store and retrieve data quickly, which is crucial in applications like databases, caches, and symbol tables.

3. Collisions Handling: Hash tables provide mechanisms to handle collisions (i.e., when two different keys produce the same hash). This ensures that data remains intact and retrievable, even in scenarios where hash values collide.

---

## WHAT - Understanding Hash Tables:

Now, let's dive into what hash tables are:

A hash table is a data structure that stores key-value pairs. It consists of an array (or a list) and a hash function. Here's how it works:

* Key: You have some data you want to store or retrieve, and each piece of data has a unique identifier called a key.

* Hash Function: A hash function takes a key as input and produces a unique index (or location) within the array where the associated value will be stored. It should distribute keys uniformly across the array to minimize collisions.

* Array: Hash tables have an array of fixed size. Each element of this array is called a bucket, and it can store multiple key-value pairs or simply a reference to a linked list or another data structure containing the key-value pairs.

---

## HOW - Implementing Hash Tables:

Now, let's discuss how to implement a basic hash table:

1. Initialize the Array: Create an array of a fixed size. The size of this array depends on your specific application and the expected number of key-value pairs to be stored.

2. Hash Function: Design a hash function that takes a key and returns an index within the array. The hash function should be deterministic (same input produces the same output) and distribute keys uniformly.

3. Insertion: To insert a key-value pair, apply the hash function to the key to find the index in the array. If there's a collision (two keys map to the same index), you can use techniques like chaining (each bucket is a linked list of key-value pairs) or open addressing (search for the next available slot).

4. Retrieval: To retrieve a value, apply the hash function to the key to find the index, then search for the value within the bucket at that index.

5. Deletion: To delete a key-value pair, use the hash function to find the index and then remove the pair from the bucket.

It's essential to choose an appropriate hash function and handle collisions effectively to ensure the hash table's efficiency and reliability.

Remember that hash tables are widely used in programming languages, databases, and many real-world applications. They provide a powerful way to store and retrieve data efficiently.

---

## Methods

**set()**
When adding a new key/value pair to a hashtable:
send the key to the hash() method.
Once you determine the index of where it should be placed, go to that index
Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
If something does exist, add the new key/value pair to the data structure within that bucket.

**get()**
The get() method takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.

**has()**
The has() method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the hash() method and check the hashtable if the key exists in the table given the index returned.

**keys()**
The keys() method returns a collection (array) of unique hash keys.

**hash()**
The hash() method will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.