#include <stdio.h>
#include <unistd.h>
int main() { 
int pid; 
pid = fork(); 
if (pid < 0) {
printf("Fork failed!\n");
} else if (pid == 0) {
printf("This is the child process. PID = %d\n", getpid());
} else {
printf("This is the parent process. PID = %d, Child PID = %d\n", getpid(), pid);
}
return 0;
}
