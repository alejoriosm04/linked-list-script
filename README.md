<h1 align = "center">Linked List Script ⛓️</h1>
<h2>
    About project
</h2> 

<p>
    This script was created for my Data Structure and Algorithms 1 class, to be able to see how our code works when we modify Linked Lists in Python and understand their behavior.
</p>

<h2>
    How does it work?
</h2> 

<p>
    This Python script will allow you to see your Linked List in the console. Also, create a new Linked List form zero and receive the output of your modifications. Importing the file that is stored in your work folder on your main file, you will be able to create a link between the functions and Classes that <code>linkedLists.py</code> has on it with your main file.
</p>
<h2>
  How to use it?
</h2>
<p>
    Clone the file <code>linkedLists.py</code> on your work folder, in the same folder where you are working with your main file.
</p>
<p>
    1. On your main file, import all the information (Classes and Functions) that <code>linkedLists.py</code> has with:
    
```python
from linkedLists import *
```
</p>
<p>
    2. Write the function that you are trying to create after import. 

```python
from linkedLists import *


def insertarAlInicio(head: Node, valor: int) -> Node:
    nuevoNodo = Node(valor)
    nuevoNodo.next = head
    return head
```
</p>
<p>
    3. In the main function, create the tests that you need to check. With the function <code>insertAtEnd(head, val)</code> you will be able to create the Nodes of your original linkedList. Remember to assign the values to the head of the Linked List. The linked list should start with <code>None</code>.

```python
from linkedLists import *


def insertarAlInicio(head: Node, valor: int) -> Node:
    nuevoNodo = Node(valor)
    nuevoNodo.next = head
    return head


def main():
    head = None
    head = insertAtEnd(head, 1)
    head = insertAtEnd(head, 2)
    head = insertAtEnd(head, 99)
    head = insertAtEnd(head, 4)
    head = insertAtEnd(head, 5)

    head = insertarAlInicio(head, 1)
    printll(head)


if __name__ == '__main__':
    main()
```
</p>
<p>
     Assign the head again, depending on the behaviour of the function that you created. If the function return a Node or a head, you have to assign this function to the head again. If the function return a value like a number or another thing different from a Node, you have to put the function inside a print to see the result. This will depend on your necessities.
</p>
<p>
    4. Finally to see your final linked List, use the function printll(head). And you will see your Linked List on your console.
</p>
<h2>
    Contribute
</h2>
<p>
    If you want to contribute to this project, do not doubt on doing a <code>Pull Request</code> for this project. I will take a look at it.
</p>
<p>
    If you have any questions or complaints please let me know.
</p>