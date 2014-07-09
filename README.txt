doubly_linked_list
==================

This code impliments a doubly linked list implimented in Python. I needed it 
for a very narrow scope, so the functionality might not have what you're 
looking for. If you'd like a feature added, please email AWNystrom@gmail.com

INSTALLATION
To instal, run the following command:
python setup.py install

TESTING
To run unit tests, run the following command:
python doubly_linked_list/test_doubly_linked_list.py

USAGE
Here's some example usage:

>>> from doubly_linked_list import DoublyLinkedList
>>> dll = DoublyLinkedList(range(10))
>>> print dll
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
>>> dll.moveToHead(dll.tail)
>>> print dll
[9, 0, 1, 2, 3, 4, 5, 6, 7, 8]
>>> dll.removeHead()
>>> print dll
[0, 1, 2, 3, 4, 5, 6, 7, 8]
>>> from random import shuffle
>>> shuffle(dll)
>>> print dll
[1, 4, 0, 2, 6, 3, 5, 7, 8]
>>> dll.moveToHead(dll.getNodeByIndex[4])
>>> print dll
[6, 1, 4, 0, 2, 3, 5, 7, 8]
