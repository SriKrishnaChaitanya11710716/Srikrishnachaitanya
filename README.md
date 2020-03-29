
CSE316: OPERATING SYSTEMS
ACADEMIC TASK -2

NAME: SRI KRISHNA CHAITANYA
REG.ID:11710716
EMAIL: srikrishnachaitanya1999@gmail.com
GitHub Link: https://github.com/SriKrishnaChaitanya11710716/Srikrishnachaitanya/blob/master/cse316


PROBLEM: 
Sudesh Sharma is a Linux expert who wants to have an online system where he can handle student queries. Since there can be multiple requests at any time he wishes to dedicate a fixed amount of time to every request so that everyone gets a fair share of his time. He will log into the system from 10am to 12am only. He wants to have separate requests queues for students and faculty. Implement a strategy for the same. The summary at the end of the session should include the total time he spent on handling queries and average query time.

PROBLEM EXPLAINATION:
•	Sudesh Sharma wants a online system that can handle student queries
•	We have multiple requests and he wishes to dedicate a fixed amount of time for every request
•	He wants to have separate requests queues for students and faculty.
•	At the end of section should include the “Total time he spent on handling queries” and “Average query time”.

SOLLUTION  PROPOSED FOR THE PROBLEM:
•	The given problem is based upon solving queries of persons of different classes i.e. Faculty and Students. Thus, these queries can be compared to different processes in terms of operating system where each process has its demands and needs resources and time for its execution.
•	 And this demands of processes are handled by the CPU. In the given scenario, Mr. Sudesh Sharma, Linux expert, can be considered as a CPU, who solves the queries of either Faculty or Student by allocating proper resources to their individual demands and processing them by allocating them time accordingly.
•	 Now, Mr. Sharma, wants to provide priority for each query based upon its class, as well as, he wants to dedicate a fixed amount of time to every request. 
•	Thus in Operating System, if we divide the requests into two separate queues i.e. Faculty and Student such that the first queue contains faculty queries has higher priority and the second contains student queries which has lower priority, then we can resolve the problem, by allocating them required resources based upon their priorities as done in the scheduling algorithm in operating systems.
•	Simply, We require “Round Robbin algorithm”  for the Problem…

DISCRIPTION:
•	“Round Robin Scheduling” is a scheduling algorithm used by the system to schedule CPU utilization. 
•	This is a preemptive algorithm. There exist a fixed time slice associated with each request called the quantum.
•	 The job scheduler saves the progress of the job that is being executed currently and moves to the next job present in the queue when a particular process is executed for a given time quantum.
•	No process will hold the CPU for a long time. The switching is called a context switch. It is probably one of the best scheduling algorithms. 
•	The efficiency of this algorithm depends on the quantum value.
 

ALGORITHM:
•	We first have a queue where the processes are arranged in first come first serve order.
•	A quantum value is allocated to execute each process.
•	The first process is executed until the end of the quantum value. After this, an interrupt is generated and the state is saved.
•	The CPU then moves to the next process and the same method is followed.
•	Same steps are repeated till all the processes are over.
COMPLEXITY:
•	O(n) Complexity. “n is the no. of  flows being sheduled”.

CONCLUSION:
•	So,for this problem we use Round Robbin Algorithm, because as we see in problem  he wants the process should execute or process for some constant time i.e, quantum time.
•	So from the code , I have allocated individual system like user can select the process is of faculty or the student
.
REFERENCES:
•	https://www.coursehero.com/file/p5567ca/All-the-processes-in-second-level-queue-will-complete-their-execution-according/
•	https://www.guru99.com/round-robin-scheduling-example.html


