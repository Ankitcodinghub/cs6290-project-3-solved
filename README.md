# cs6290-project-3-solved
**TO GET THIS SOLUTION VISIT:** [CS6290 Project 3 Solved](https://www.ankitcodinghub.com/product/cs-6290-high-performance-computer-architecture-solved-3/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;126109&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS6290 Project 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
&nbsp;

This project is intended to help you understand cache coherence and performance of multicore processors. As with previous projects, for this project you will need VirtualBox and our project virtual machine. Just like in previous projects, you will put your answers in the reddish boxes in this Word document, and then submit it in Canvas (but this time the submitted file name should be PRJ3.docx).

Additional files to upload are specified in each part of this document. Do not archive (zip, rar, or anything else) the files when you submit them, except when we explicitly ask you to submit a zip file (in Part 3H). Each file we are asking for should be uploaded separately, and its name should be as specified in this assignment. You will lose up to 20 points for not following the file submission and naming guidelines. Furthermore, if it is not VERY clear which submitted file matches which requested file, we will treat the submission as missing that file. The same is true if you submit multiple files that appear to match the same requested file (e.g. several files with the same name). In short, if there is any ambiguity about which submitted file(s) should be used for grading, the grading will be done as if those ambiguous files were not submitted at all.

Most numerical answers should have at least two decimals of precision. Speedups should be computed to at least 4 decimals of precision, using the number of cycles, not the IPC (the IPC reported by report.pl is rounded to only two decimals). You lose points if you round to fewer decimals than required, or if you truncate digits instead of correctly rounding (e.g. a speedup of 3.141592 rounded to four decimals is 3.1416, not as 3.1415).

username here

This project can be done either individually or in groups of two students. If doing this project as a two-student group, you can do the simulations and programming work together, but each student is responsible for his/her own project report, and each student will be graded based solely on what that student submits. Finally, no collaboration with other students or anyone else is allowed. If you do have a partner you have to provide his/her name here (enter None here if no partner) and his/her Canvas . Note that this means that you you cannot change partners once you begin working on the project, i.e. if you do any work with a partner you cannot “drop” your partner and submit the project as your own (or start working with someone else) because the collaboration you already had with your (original) partner then becomes unauthorized collaboration.

Part 1 [40 points]: Running a parallel application

In this part of Project 3 we will be using the LU benchmark. We will also be using a processor with more (sixteen) cores (cmp16-noc.conf). So, for example, to simulate 4threaded execution you would use a command like this (note the absence of spaces between -n and 512, and between -p and 4):

~/sesc/sesc.opt -fAp4 -c ~/sesc/confs/cmp16-noc.conf -olu.out -elu.err lu.mipseb -n512 -p4 To complete this part of the project, run the lu application with 1, 4, and 16 threads. Then fill in the blanks, taking into account all the runs you were asked to do:

A) Submit the three simulation reports: sesc_lu.mipseb.Ap1, sesc_lu.mipseb.Ap4, and sesc_lu.mipseb.Ap16. You will not earn points for submitting these simulation reports, but you will lose 10 points for each missing simulation report.

B) Fill out the execution time, parallel speedup, and parallel efficiency with 4 and 16 threads. Enter Sim Time with precision of at least three decimals, and speedup and efficiency with precision of at least two decimals.

Note: Parallel speedup is the speedup of parallel execution over the single-thread execution with the same input size. Parallel efficiency is the parallel speedup divided by the number of threads used – ideally, the speedup would be equal to the number of threads used, so the efficiency would be 1. When computing the speedup and efficiency we cannot use IPC or Cycles that are reported for each processor, because these do not account for the cycles where that core was idle (e.g. because the thread was waiting for something to happen). So we need to use the “Sim Time” we get from report.pl because it accounts for all cycles that elapse between the start and completion of the entire benchmark.

C) Our results indicate that parallel efficiency changes as we use more cores. Why do you think this is happening?

Synchronization between threads especially when accessing a shared memory or shared cache can cause the parallel efficiency changes. The more cores there are the more synchronization needs to happen so a core doesn’t get outdated values or information from memory or cache. With 1 core, it doesn’t need synchronization because its running on a single thread and doesn’t need to share with anyone.

D) When we use four threads (-p4) instead of one (-p1), the IPC achieved by Core 0 (the first processor listed) got slightly lower because

Core 0 is main thread so there’s less work for it to do meaning less IPC, more delegating work to the other 3 worker threads. After that’s done, it probably waits for the worker threads to finish up and as a result spends most of its time just waiting. The more waiting it does, the lower the IPC of the core 0.

E) Now look at the simulation reports for these simulations. Core 0 executes more than its fair share of all instructions because

Core 0 is the main thread, has to set up the other threads for the other cores, and need to give them instructions on what to do. Even though IPC is lower, a good number of instructions are still needed to delegate work to the other worker threads/cores on the processor and after delegating it still needs to clean up and close those threads properly.

Part 2 [10 points]: Cache miss behavior

In this part of Project 3, we will be focusing on the number of read misses in the DL1 (Data L1) cache of Core 0, using the same simulations that we already did for Part 1. In the report file generated by the simulator (sesc_lu.mipseb.something, not what you get from report.pl), the number of cache read misses that occur in each DL1 cache (one per processor core) is reported in lines that begin with “P(0)_DL1:readMiss=”.

F) The total number of read misses that occur in the DL1 cache of Core 0 is

Simulation -p1 -p4 -p16

Core 0’s

DL1 read misses 760977

C 220878

C 78308

C

Your answers here should be integer numbers.

G) The number of these misses changes this way as we go from one to two to four, etc. threads because

Core 0 is the main thread mostly in charge of creating worker threads, and the main thread doesn’t need as much memory accesses, therefore less cache miss. With more cores, the memory accesses are more spread out too among the cores, leading a decrease in misses.

Part 3 [50 points]: Identifying accesses to shared data

H) Create a Changed.zip file with any simulator source code files that you have modified in Part 3 of the project, and submit this Changed.zip file together with your project. You will not earn points for submitting this file, but you will lose 50 points if it is missing or if it does not contain all the source code modifications. Then, with your changed simulator (that now counts compulsory, replacement, and coherence read misses), re-run the simulations from Part 1 and submit the resulting simulation report files as sesc_lu.mipseb.Hp1, sesc_lu.mipseb.Hp4, and sesc_lu.mipseb.Hp16. As in Part 1, you will not earn points for these submitted simulation reports, but you will lose 10 points for each simulation that is missing.

I) The number of all read misses, compulsory read misses, replacement read misses, and coherence read misses for the DL1 cache of Core 0 is:

Core 0’s DL1 Core 0’s DL1 Core 0’s DL1 Core 0’s DL1 readMiss compMiss replMiss coheMiss

760977 122 760855 0

-p1 C C C C

126 220629 123

-p4 220878 C C C C

78308 134 77861 313

-p16 C C C C

Note: readMiss numbers here should be the same as those you had in Part 2.

J) The number of all write misses, compulsory write misses, replacement write misses, and coherence write misses for the DL1 cache of Core 0 is:

Core 0’s DL1 Core 0’s DL1 Core 0’s DL1 Core 0’s DL1 readMiss compMiss replMiss coheMiss

33056 32981 75 0

-p1 C C C C

33319 33018 80 221

-p4 C C C C

33672 33156 78 438

-p16 C C C C
