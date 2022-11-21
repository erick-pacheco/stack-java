# Instructions  
### Description:
A stack is a data structure that adheres to the “last in, first out”, or LIFO, method of processing elements. The last element of a stack is referred to as the “top” of the stack. When adding or removing from a stack, you start at the top.

Common stack operations:
* push: add to the end of the data structure
* pop: remove from the end of the data structure
* peek: get the last element in the data structure

There are two Java classes that can be used to implement the Stack data structure: the Stack class and the ArrayDeque class. It is recommended to use the ArrayDeque class over the Stack class to implement a Stack. This is because the Stack class is considered legacy, or outdated: it allows for accessing elements using an index, which is not typical of a stack data structure, and it performs slower than a stack implemented with ArrayDeque.

In this activity you will be learning about how to create and use a stack in Java. Please follow the steps below:

### Steps:
1. Add the following code inside of the **main()** method:
```Java
 ArrayDeque<String> stack = new ArrayDeque<>();
```
The statement we added creates an ArrayDeque, a subtype of Queue, and assigns it to a corresponding reference variable. This queue will be used as a stack and can store String objects.

2. Now that we have a stack to work with, let's add some elements to it. Add the following code inside of the **main()** method, below any code you have in it so far:
```Java
stack.push("Apple");
stack.push("Banana");
stack.push("Cherry");
```
The **push()** method adds to the stack. Elements are added to the end or "top" of the stack.

3. Next, let's see what the first element in the queue is. Add the following code inside of the **main()** method, below any code you have in it so far:
```Java
System.out.println(stack.peek());
```
The **peek()** method returns the value of the last element in the stack. The output to the console should be `Cherry`.

4. Now it's your turn. Create a stack that will hold Integer objects.
2. Use a loop to add the values `0 - 10` to the stack.
3. Create a while loop that will iterate over your collection. The loop should keep running as long as the collection is not empty. You may want to use the **isEmpty()** method that collections have.
4. For every iteration of the loop, remove and print out the current top element using the **System.out.println()** and **pop()** method.
5. Run the program. Notice how the stack pops out the last item as the first. This is called LIFO (Last in first out).

### Test:
Use the test provided. 

#### Sample output:
```
Cherry
10
9
8
7
6
5
4
3
2
1
0
```