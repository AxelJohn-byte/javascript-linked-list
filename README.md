# javascript-linked-list

This program uses two JavaScript classes to build and display a linked list on a webpage.

The ListNode class creates the individual building blocks. Each node stores two things: the piece of data itself (like "Apple") and a pointer called next that starts as null. This next pointer is what attaches one node to the next in a sequence.

The LinkedList class manages the full chain of nodes. It starts with a head variable set to null. The head acts as the front door—it always points to the very first node in the list so the program knows where to begin.

When you add a new item using add(data), the program first creates a new ListNode. If the list is empty (head is null), head points directly to this new node. If items already exist, the program uses a temporary variable to walk through the chain step-by-step (current = current.next) until it finds the last node. It then attaches the new node to the last node's next pointer.

Finally, the display() method reads the entire list. Starting at head, it moves node by node, collecting each piece of text into a single string. Once it reaches the end of the list, it finds the <p id="output"> tag in the HTML document and sets its content to display Apple Banana Orange  on the page.
