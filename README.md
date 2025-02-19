# Go Race Condition in Goroutine with Mutex

This repository demonstrates a race condition in a Go program that uses goroutines and a mutex to protect a shared variable. The race condition can cause unexpected results, and this repository shows how to fix it. 

## Bug Description

The program uses 1000 goroutines to increment a shared variable x. A mutex is used to protect the variable from race condition, however, this implementation is still buggy.  The issue lies in how the goroutines access the shared variable concurrently despite the mutex. 

## Solution

The solution involves making sure that the mutex is used correctly in protecting the shared variable.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/go-race-condition.git
   ```
2. Navigate to the repository directory:
   ```bash
   cd go-race-condition
   ```
3. Run the program:
   ```bash
   go run bug.go
   go run bugSolution.go
   ```