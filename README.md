# inheritance-CS50x

This is a C program that simulates the inheritance of blood types for each member of a family

## Problem Statement

The program simulates the inheritance of blood types for multiple generations within a family. Each person has two alleles (A, B, or O) that determine their blood type. The program randomly assigns alleles to each person, following the rules of genetic inheritance.

## Getting Started

To run the program, follow these steps:

1. Open your terminal.

2. Navigate to the directory where you want to clone the repository.

3. Clone the repository using the following command:

   ```
   git clone https://github.com/MONISHSHARMA080/inheritance-CS50x.git
   ```
4. Compile using
   ``` make inheritance```

5.Run the program:
  ```./inheritance```
  
## Background
A person's blood type is determined by two alleles, which can be one of three types: A, B, or O. Each person inherits one allele from each parent, resulting in various possible blood type combinations. For example, if one parent has blood type AO and the other has blood type BB, their child's possible blood types would be AB and OB, depending on which allele is inherited from each parent.

### Implementation Details
The inheritance.c file contains the main program logic. The key functions to complete are create_family and free_family.

create_family Function
This function creates a family of a specified generation size and assigns blood type alleles to each family member. The oldest generation has alleles assigned randomly.

Input: An integer generations representing the number of generations in the family.

Output: A pointer to the person in the youngest generation.

free_family Function
This function accepts a pointer to a person as input, frees memory for that person, and recursively frees memory for all of their ancestors.

Input: A pointer to a person.

Output: Frees memory for the entire family tree.
## Example 
```$ ./inheritance
Child (Generation 0): blood type OO
    Parent (Generation 1): blood type AO
        Grandparent (Generation 2): blood type OA
        Grandparent (Generation 2): blood type BO
    Parent (Generation 1): blood type OB
        Grandparent (Generation 2): blood type AO
        Grandparent (Generation 2): blood type BO```
