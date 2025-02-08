# OS Project - Banker's Algorithm

## Overview
This project implements the **Banker's Algorithm**, which is used in operating systems to avoid deadlock and ensure safe resource allocation. The algorithm checks whether the system is in a safe state before allocating resources to processes.

## Features
- Accepts user input for the number of resources and processes.
- Takes allocation and maximum demand matrices as input.
- Computes the **Need Matrix** (Max - Allocation).
- Determines if the system is in a **safe state**.
- Prints the **safe sequence** if the system is in a safe state.

## Input Requirements
- **Number of resources** (Maximum of 5)
- **Instances of each resource**
- **Number of processes** (Maximum of 10)
- **Allocation Matrix** (Current allocation of resources to each process)
- **Max Matrix** (Maximum resource demand of each process)

## How It Works
1. Accepts input values for resources and processes.
2. Calculates the available resources after allocation.
3. Computes the need matrix by subtracting the allocation from the max demand.
4. Runs the Banker's Algorithm to check system safety.
5. If a safe sequence exists, it is printed; otherwise, an unsafe state is reported.

## Usage
1. Compile the program using a C++ compiler:
   ```sh
   g++ OS_PROJECT_CODE.cpp -o bankers_algorithm
   ```
2. Run the executable:
   ```sh
   ./bankers_algorithm
   ```
3. Follow the on-screen instructions to input resource and process details.

## Example Output
```
Enter the number of resources (<=5): 3
Enter the max instances of resource R[0]: 10
Enter the max instances of resource R[1]: 5
Enter the max instances of resource R[2]: 7
Enter the number of processes (<=10): 5
Enter the allocation matrix:
...
The system is in a safe state.
Safe sequence is: P[1] -> P[3] -> P[0] -> P[2] -> P[4]
```

## License
This project is open-source and free to use.

## Author
Developed as part of an **Operating Systems** project.

