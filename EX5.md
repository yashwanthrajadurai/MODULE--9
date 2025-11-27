## Ex.No:5

## Ex.Name: Write the preOrder Traversal module of splay tree in CPP.

## Aim:
To write the preOrder Traversal module of splay tree in CPP.

## Algorithm:
1. Start from the root node.
2. Visit (print) the current node.
3. Traverse the left subtree.
4. Traverse the right subtree.
5. Repeat recursively for all nodes until entire tree is visited.

## Program:
```
void preOrder(struct node *root)
{
    if(root!=NULL)
    {
        cout<<root->key<<" ";
        preOrder(root->left);
        preOrder(root->right);
    }
    
}
```


## Output:
<img width="1184" height="616" alt="Screenshot 2025-11-16 105423" src="https://github.com/user-attachments/assets/3f0b4ff7-c929-4526-b50d-31f30a810bb2" />

## Result:
Thus the program created susseccfully to preOrder Traversal module of splay tree in CPP.
