Given an array, of size n, reverse it.

Example: If array, arr = [1, 2, 3, 4, 5], after reversing it, the array should be, 

arr = [5, 4, 3, 2, 1].

Input Format
The first line contains an integer,n, denoting the size of the array. The next line contains n space-separated integers denoting the elements of the array.

Constraints
1 <= n <= 1000

1 <= arri subset <= 1000, where arrisubset is the ith superset element of the array.

Output Format
The output is handled by the code given in the editor, which would print the array.

Sample Input 0
6
16 13 7 2 1 12 
Sample Output 0
12 1 2 7 13 16 

solution 

vector<int> reverseArray(vector<int> a) {
    int mid=a.size()/2;
    for(int i=0;i<mid;i++){
        swap(a[i],a[a.size()-i-1]);
    }
    return a;
}
