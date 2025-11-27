## Ex.No:4

## Ex.Name: Write the search Module of B Tree in CPP.

## Aim:
To write the search Module of B Tree in CPP

## Algorithm:
1. Start from the root node.
2. Find the smallest index i such that key ≤ node->keys[i].
3. If key == node->keys[i], return node (key found).
4. If node is a leaf, return NULL (key not found).
5. Otherwise, move to the child pointer node->children[i].
6. Repeat the process recursively until key is found or leaf is reached.

## Program:
```
void search(int val, int *pos, BTreeNode *myNode) 
{
    if (!myNode) 
    {
    return;
    }

    if (val < myNode->val[1]) 
    {
        *pos = 0;
    }
    else
    {
        for (*pos = myNode->count;(val < myNode->val[*pos] && *pos > 1); (*pos)--);
        if (val == myNode->val[*pos]) 
        {
            cout<<"Element "<<val<<" found";
        }
    }
    search(val, pos, myNode->link[*pos]);
    return;
}
```


## Output:
<img width="1190" height="456" alt="Screenshot 2025-11-16 105134" src="https://github.com/user-attachments/assets/e13016dd-c90c-495f-b661-b7838c263635" />

## Result:
Thus the program created successfully to search Module of B Tree in CPP.

