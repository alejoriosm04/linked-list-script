<h1 align = "center">Linked List Script ⛓️</h1>

Script that tests the behavior of linked lists in Python.

Created for the course _Data Structures and Algorithms I_ at [EAFIT University](https://github.com/eafit/).


## What it does

- Links the functions and classes of `linkedLists.py` with your main file
- Prints your linked list in the console
- Create a linked list from scratch and see the output from your modifications


## Examples

In `/examples` path you will find some implementations.

There is also a `template.py` to adapt your main file.

## Step-by-step guide

Clone the script `linkedLists.py` on your work folder (where your main file is).

**Do ***not*** modify** the script. All the tests will actually be within your main file.

1. Import the classes and functions of `linkedLists.py` _on your main file_:
    
```python
from linkedLists import *
```

2. Code the function you want to test _on your main file_:

```python
def insertarAlInicio(head: Node, valor: int) -> Node:
    nuevoNodo = Node(valor)
    nuevoNodo.next = head
    return head
```

3. In the `main()` function, create the tests to check for.

The `insertAtEnd(head, val)` function (from the script) creates the Nodes of your original linked list

Remember to assign the values to the head of the linked list. Also, it must begin with `head = None`.

```python
def main():
    head = None
    head = insertAtEnd(head, 1)
    head = insertAtEnd(head, 2)
    head = insertAtEnd(head, 99)
    head = insertAtEnd(head, 4)
    head = insertAtEnd(head, 5)
    # 5->4->99->2->1->None

    head = insertarAlInicio(head, 1)
```

<!---
I still find this paragraph very confusing...
-->
When you are going to use your function, assign the head again, depending on the behavior of the function that you created. If the function return a Node or a head, you have to assign this function to the head again. If the function return a value like a number or another thing different from a Node, you have to put the function inside a print to see the result. This will depend on your necessities.

4. Run the `printll(head)` function to print your modified linked list.

```python
printll(head)
# PENDING: OUTPUT AFTER
```


## Contribute

Pull requests are welcome. I will take a look at them.
