---
title: "Parallel Computing Technique using OpenMP"
excerpt: |
    This repository explores various techniques to optimize matrix multiplication wall time using OpenMP, a shared-memory multiprocessing API. The study compares serial execution, parallel execution with OpenMP, and optimized parallel execution, aiming to enhance computational performance in multi-threaded environments.
    
    <br/> <center>
    <img src='/images/portfolio/Optimized_Parallel_Execution_grpah.png' alt='Matrix Multiplication Program Interface' style='width: 400px; display: block; margin: auto;'>
    </center>
    <br/>
    <div>
        <p><strong>Key Techniques:</strong></p>
    <ul>
        <li><strong>Serial Execution:</strong> Executes matrix multiplication sequentially in a uniprocessor system.</li>
        <li><strong>Parallel Execution with OpenMP:</strong> Utilizes OpenMP for multi-threaded matrix multiplication.</li>
        <li><strong>Optimized Parallel Execution:</strong> Improves performance through memory access optimization and compiler flags.</li>
    </ul>
    </div>
collection: portfolio
---

## Overview 🌐
Matrix Multiplication Execution Techniques using OpenMP is a comprehensive project that evaluates the performance of different matrix multiplication methods. By leveraging the power of parallel processing, the project seeks to minimize computational time and enhance efficiency.

## How It Works 🧐
The project examines three execution strategies for matrix multiplication—serial, parallel with OpenMP, and optimized parallel—to determine the most effective approach for reducing wall time in computation-heavy tasks.

## Main Techniques 🔥
- **🔢 Serial Execution**: The baseline for performance comparison, running operations in sequence.
- **🚀 Parallel Execution with OpenMP**: Exploits the parallelism offered by OpenMP, distributing tasks across multiple processors.
- **⚙️ Optimized Parallel Execution**: Focuses on compiler optimizations to further reduce computation time.

<a href="https://github.com/mdalmaruf/ParallelComputingOpenMP.git" style="color:#52adc8;"><strong>View the project on GitHub ![GitHub](/images/icons8-github-30.png)</strong></a>

## Experimental Analysis 📊
The project includes a thorough experimental setup and detailed result analysis to compare the execution times across different methods. The study provides insights into the benefits of parallelization and optimization in computational tasks.

![Serial vs. Parallel Execution Comparison Graph](Data/ParallelExecution.PNG)

*Figure 1: Serial vs. parallel execution comparison*

![Execution Time with Various Compiler Optimizations](Data/Optimized_Parallel_Execution_graph.png)

*Figure 2: Execution time with No Compiler Optimization vs. Aggressive Compiler Optimization*

## Findings and Contributions ✨
The findings indicate significant improvements in execution times with parallel and optimized techniques. For a full understanding of the methods and results, the project report is available with detailed graphs and performance analysis.

We welcome contributions and suggestions for further optimizations and enhancements to the project.
