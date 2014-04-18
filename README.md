Distributed-Hash-Table
======================

Simple Key-Value storage based on Chord design.
Simplified version of Chord, covers three things:

ID space partitioning/re-partitioning.
Ring based routing
Node joins
SHA-1 hash function is used to lexically arrange nodes in a ring and find the location for a particular key to be stored.

Each node maintains a successor and predecessor pointer for nodes in the ring.
Content Provider is NoSQL storage that:

The first column should be named as “key”. This column is used to store all keys.
The first column should be named as “value”. This column is used to store all values.
However, Node failures, concurrent node-joins and finger tables are not implemented.

PTest

Inserts 50 arbitrary key-value pairs in the DHT and queries to check if they exist and returns success/failure messages.

References

[1] Read about Chord here

[2] Single best resource on Android, Android dev

[3] Link to Chord repository on Github, here
