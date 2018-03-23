# semaphore-class


1. What are the main differences between *message passing* and *shared memory* in inter-process communication? Describe and contrast.  

2. Consider the following functions that will execute as threads: 

   ```cpp void \*threadA ( void *ptr )**
   void *threadA ( void *ptr )
   {
       printf("Statement A \n");
       fflush(stdout);
       pthread_exit(0); 
   }

   void *threadB ( void *ptr )
   {
       printf("Statement B \n");
       fflush(stdout);
       pthread_exit(0); 
   }

   void *threadC ( void *ptr )
   {
       printf("Statement C \n");
       fflush(stdout);
       pthread_exit(0); 
   }
   ```

   Write a program that uses semaphores to serialize the 3 threads. The correct sequence of statements should be: B, C, A. 
