## [Reflection](#Reflection)<br>

---

### Pre-Profiling and Optimization Tests

/all-student JMeter GUI test Pre-Profiling
![all-student pre-profiling.png](./Test_Results/all-student%20pre-profiling.png)

/all-student-name JMeter GUI test Pre-Profiling
![all-student-name pre-profiling.png](./Test_Results/all-student-name%20pre-profiling.png)

/highest-gpa JMeter GUI test Pre-Profiling 
![highest-gpa pre-profiling.png](./Test_Results/highest-gpa%20pre-profiling.png)

/all-student JMeter CLI test Pre-Profiling
![all-student pre-profiling.png](./Test_Results/all-student%20pre-profiling%20JTL.png)

/all-student-name JMeter CLI test Pre-Profiling
![all-student-name pre-profiling JTL.png](./Test_Results/all-student-name%20pre-profiling%20JTL.png)

/highest-gpa JMeter CLI test Pre-Profiling
![highest-gpa pre-profiling JTL.png](./Test_Results/highest-gpa%20pre-profiling%20JTL.png)


### Post-Profiling and Optimization Tests

/all-student JMeter GUI test Post-Profiling
![all-student post-profiling.png](./Test_Results/all-student%20post-profiling.png)

/all-student-name JMeter GUI test Post-Profiling
![all-student-name post-profiling.png](./Test_Results/all-student-name%20post-profiling.png)

/highest-gpa JMeter GUI test Post-Profiling
![highest-gpa post-profiling.png](./Test_Results/highest-gpa%20post-profiling.png)

/all-student JMeter CLI test Post-Profiling
![all-student post-profiling.png](./Test_Results/all-student%20post-profiling%20JTL.png)

/all-student-name JMeter CLI test Post-Profiling
![all-student-name post-profiling JTL.png](./Test_Results/all-student-name%20post-profiling%20JTL.png)

/highest-gpa JMeter CLI test Post-Profiling
![highest-gpa post-profiling JTL.png](./Test_Results/highest-gpa%20post-profiling%20JTL.png)

---

### Conclusion
After implementing profiling and performance optimizations, a significant improvement was observed across all test cases. 
The JMeter results show substantial reductions in execution time:

1. **All Students API**
    
    Before Profiling: 90,000 - 91,000 ms

    After Profiling: 3,900 - 4,100 ms

    Improvement: ~95% reduction in execution time <br><br>

2. **All Student Names API**

    Before Profiling: 3,000 - 4,000 ms

    After Profiling: 90 - 100 ms

    Improvement: ~97% reduction in execution time <br><br>

3. **Highest GPA API**

    Before Profiling: 80 - 85 ms 
    
    After Profiling: 6 - 7 ms
    
    Improvement: ~92% reduction in execution time


The optimizations, including query optimizations, repository improvements, and better data handling, led to a drastic reduction in response times. 
The most significant gains were in the all-student and all-student-name endpoints, where response times decreased by nearly 95-97%. 
Even the highest-GPA query, which was already relatively fast, saw a 92% improvement.

These results highlight the critical importance of profiling and optimizing code in achieving optimal system performance. 
By identifying bottlenecks and refining database queries and data retrieval strategies, we were able to significantly reduce execution times. 
This demonstrates that regular performance profiling and targeted optimizations are essential for maintaining scalable and efficient applications.

---

## Reflection

1. **What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?**

   JMeter tests system-level performance, while IntelliJ Profiler diagnoses performance bottlenecks at the code level. <br><br>
   
2. **How does the profiling process help you in identifying and understanding the weak points in your application?**

   Profiling helps by, Locating slow methods, Detecting memory leaks, Analyzing database queries, and Identifying thread issues <br><br>
   
3. **Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?**

   IntelliJ Profiler is effective in assisting me to analyze and identify bottlenecks in my application code because
   it provides real-time monitoring of CPU, memory, and execution time while also allows call tree analysis to track how methods contribute to execution time <br><br>
   
4. **What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?**

   Identifying the cause of the slow performance can be a challenge, especially for a beginner like me, 
   I overcame it by following the tutorial and implementing what I learnt on the other 2 tests <br><br>
   
5. **What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?**

   Pinpointing inefficient code at the method level and providing real-time CPU and memory usage insights  <br><br>
   
6. **How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter?**

    I would cross-check findings, consider environmental factors, and re-run tests with different conditions (to identify variable factors) <br><br>
   
7. **What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?**

    I refactored inefficient codes and optimize database queries. Of course, I did not change the functionality of my code because I refactored the code and not modified it. <br><br>

---
