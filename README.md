# oop_Assignment_2

 #### This is the third assignment of oop , in this assignment we have implemented and used few of the design patterns that we have learnd    through the semester, such as the: Observer , Adapter , Factorial. very important design patters which are used world-wide.



## First part of the assignment.
in this part we were requierd to make a class named Ex_2 which conatins total of 4 methods: 
createTextFiles , getNumOfLines , getNumOfLineThread and getNumOfLinesThreadPool.

1. **createTextFile (int n, int seed, int bound)** - the mehod creats n text files and generates a random number of lines for each and every one of them , then the method return an array size of n wich contains the names of the files.

2. **getNumOfLines(String [] fileNames)** - the method recive an array which contains names of files , the method will return the total amount of the lines of all the files.

3. **getNumOfLinesThread(String [] fileNames)** - the method receivs an array which contains names of files , the method will return the total amount of the lines of all the files using Threads.

4. **getNumOfLinesThreadPool(String [] fileNames)** - the method receivs an array which contains names of files, 
the method will return the total amount of the lines of all the files using ThreadPool.

 


### uml diagram of the class :
![WhatsApp Image 2023-01-10 at 20 53 23](https://user-images.githubusercontent.com/118810462/211641778-a463f5a1-e4ce-4d54-83c2-de62cfe1a156.jpeg)

#### MyThread 
a class that inheriate from the Thread class , implemented the run method as a method to count all the lines in a specified file.
used for the third mehod.   

#### MyThreadPool 
a class that implements the Callable class , modified the call() method so that it will return the amount of lines in a specified file. 
used for the forth method.


## Conclusions 
![WhatsApp Image 2023-01-10 at 20 21 19](https://user-images.githubusercontent.com/118810462/211872980-5a935c05-b58a-4180-9b7a-97200b602edf.jpeg)

we have tested both the ThreadPool and Threads methods and checked what is faster , as shown above in large scale of files the Threads method won the race , however they were super close. To our knowledge the reason that the Threads method won is because in this specific implementation the Threads didn't have to do deal with all the managment and the threads creation like the ThreadPool .
