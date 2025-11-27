
## Ex.No:1

## Ex.Name: Write the Search Module of the BPlus Tree in CPP.

## Aim:
To write the Search Module of the BPlus Tree in CPP

## Algorithm:
1. Start from root node.
2. Compare key with keys in current node.
3. Find the correct child pointer to follow.
4. Move to the child node.
5. Repeat until a leaf node is reached.
6. Search the key inside the leaf node.
7. If found → return success, else return not found.
   
## Program:
```
void BPTree::search(int x)
{
    if (root == NULL)
    {
    cout << "Tree is empty\n";
    }
    else
    {
        Node *cursor = root;
        while (cursor->IS_LEAF == false) 
        {
            for (int i = 0; i < cursor->size; i++)
            {
                if (x < cursor->key[i])
                {
                    cursor = cursor->ptr[i];
                    break;
                }
                if (i == cursor->size - 1) 
                {
                    cursor = cursor->ptr[i + 1];
                    break;
                }
            }
        }
        for (int i = 0; i < cursor->size; i++)
        {
            if (cursor->key[i] == x)
            {
                cout << "Found\n";
                return;
            }
         }
        cout << "Not found\n";
    }
}
```


## Output:
<img width="1100" height="763" alt="Screenshot 2025-11-16 102524" src="https://github.com/user-attachments/assets/3962caba-36cd-4977-b125-c8a3f97fc6ff" />

## Result:
Thus ths program created successfully for Search Module of the BPlus Tree in CPP.

