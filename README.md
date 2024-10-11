# HotPotato
Simulate a HotPotato Game
The Hot Potato game is a classic illustration of how queues work in real-world scenarios. In this simulation, the game is modeled by utilizing the First-In-First-Out (FIFO) nature of a queue to manage the children passing an item (the potato) around a circle. Let's break this down further:

Game Mechanics:
Players in a Queue: The players are arranged in a queue (as shown in Figure 3.13.2). The child holding the potato is at the front of the queue.

Passing the Potato: Each time the potato is passed, the child at the front of the queue is dequeued and re-enqueued at the back, simulating them handing off the potato and waiting for their next turn. This continues for a number of passes defined by the variable num.

Elimination: After num passes, the child at the front of the queue is eliminated (dequeued permanently), and the game proceeds with the remaining children. This repeats until only one child remains, who is declared the winner.

Key Concepts:
FIFO Queue: The circular nature of the game is managed by a queue, where children move from the front to the back after passing the potato.

Queue Operations:

Enqueue: Adds an element to the back of the queue.
Dequeue: Removes an element from the front of the queue.
Implementation Details:
The function hotPotato accepts a list of names (nameList) and a number (num) that determines how many times the potato is passed.

The program uses a loop to simulate the repeated passing of the potato, with the child being eliminated after every num passes.
