Disk based data structure

This is a java library for disk based datastructures to handle backpressure.
Problem

If you need very large structure like a queue or stack, whose size can be beyond your RAM or primary memory then you can use library. 
Currently if you are exceeding memory limits then your OS will start swapping between primary and secondary memory. The problem with this approach is that you cannot control how much and which data is getting swapped. This might reduce your performance. 
For a typical producer consumer based data structure like stack or queue, this might not be needed. Typically your stack or queue increases when your producers are way too fast than your consumers. In this scenario you really don't need to swap large amount of memory, you just need enough for consumers to consume at desired rate.
