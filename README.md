# Factors of a Number

## Overview
This C++ program finds and prints all the factors of a given integer.  
A factor is a number that divides the given number completely without leaving a remainder.

## How It Works
- The program reads an integer `n`.
- It creates a vector `ans` to store all factors.
- A loop runs from `1` to `n`:
  - If `n % i == 0`, then `i` is a factor.
  - The factor is stored in the vector.
- Finally, all stored factors are printed.

## Input
- A single integer value.

## Output
- All factors of the number separated by space.

## Example

Input:
12  

Output:
1 2 3 4 6 12  

## Code

```cpp
#include<bits/stdc++.h>
using namespace std;

int main(){
    int n;
    cin >> n;

    vector<int> ans;

    for(int i = 1; i <= n; i++){
        if(n % i == 0){
            ans.push_back(i);
        }
    }

    int s = ans.size();

    for(int i = 0; i < s; i++){
        cout << ans[i] << " ";
    }
}
