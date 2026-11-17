# Union find 

## What does it aim to solve
Union find is used to join disjoint objects/elements into groups. 
Useful in graph problems where certain groups need to be linked together


## General Solution 

Generally we connect each node to their parent and this is stored in a vector<int>parent. We start off with each node being its own
parent and then we travese the graph allocating the correct parent using the unite and find functions.

The find and unite function are ususally the same no matter the question:

The find function aims to find the 'root' parent. 
```cpp
find(int x){              
    if(parent[x]!= x){
        return find(parent[x]);
    }
    return parent[x];
}
```
The unite function finds the root parent of x and y and in this example joins parent x to parent y
```cpp
void unite(int x, int y){
int parentX = find(x);
int parentY = find(y);
if(parentX != parentY){
    parent[parentX] = parentY;
}
}
```

In the main function we need to init the parent to be correct size and make the parent vector equal to itself this is done with 

```cpp
std::iota(parent.begin(),parent.end(),0);
```



