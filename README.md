[IMG_1348.pdf](https://github.com/user-attachments/files/28203762/IMG_1348.pdf)
# SSU-CS-351
My computer architecture class I took at Sonoma State University  in spring of 2026

My list
*Project 1

1) Which program is fastest? Is it always the fastest?

    - In general, alloca.out has had the fastest times overall compared to all of the other programs. However, it is not always the fastest. If you were compare every single test, there are some points where malloc.out is actually faster than alloca.out. That can be seen when do min bytes & max bytes= 1000, a num block= 1000000, and num blocks 10000000

2) Which program is slowest? Is it always the slowest?
    - The program that is usually the slowest is list.out when compared overall to the other programs. It wasn't the slowest everytime though. Sometimes it was tied with new.out or new.out would actually be the slowest depending on the test that 
    was happening, similarly to alloca.out and malloc.out

3) Was there a trend in runtime based on node data size? Why?
    - Yes there was a trend when it came to node data size between alloca, list, alloc, and new because as there were increases in the min bytes and max bytes, the data became less and less distinguishable between all 4. As well as it taking a much longer time for the information to be processed and outputted. This was a especially apparent with alloca which is normally the fastest but you can see the numbers increase as the min and max bytes increased. The reason why this happens to all of them is because hashing starts to dominate the process over whats happening on the stack. 
4) Was there a trend in runtime based on block chain length?
    - Yes there was a trend in the runtime. Originally when I had tried to run the test, I found that I had forgotten to increase the amount of stack space on my 
    terminal and what ended up happening was alloca crashed! When I made stack space unlimited this didn't happen, however it took a significantly longer time and 
    that was very apparent when I was waiting for all of the results to be printed as well as when I was comparing all of the run times. Upon further research, I found that the reason why this was happening was because alloca is a recursive function which means each increase made by the block sizes is more of the stack space being used. While all of the other functions will also be doing so, making stack space dissapear even faster. All of this accounted for, it makes sense why the the runtime increased so much. 
    
5) What's noticeable about heap breaks? Does stack size affect the heap?
    - Heap breaks continue to happen as all of these functions ask for more and more stack space as it tries to accomodate their growth. Stack size and the heap go hand and hand, so they definitely affect each other and their growth.
6) Draw a two-node diagram for malloc.cpp or alloca.cpp showing pointers, node size, and structure
    - [IMG_1348.pdf](https://github.com/user-attachments/files/28203766/IMG_1348.pdf)

7) Were any allocation/init/hashing tasks the same across programs? Which differed?
    - there were a few, I think alloc and malloc had a few times and the same happened for list and new. However, when it came to the ones that differed most, those two groups almost never overlaped or came close to each other. There were a few times but, very few. 
8) As node data size grows, does allocation overhead matter more or less?
    - As data size grwos overhead matters even more, the reason why is because of the amount of hashing it takes as each node is added. I originally thought it was due to stack space, but the amount of automation it takes to do the hashing takes over even more to do. 



