
## Ex.No:2

## Ex.Name: Write the Traversal module of the red black tree in CPP.

## Aim:
To write the Traversal module of the red black tree in CPP.


## Algorithm:
1. Start from the root node.
2. Move to the left child.
3. Keep moving left until no more left child.
4. Visit (print) the current node.
5. Move to the right child.
6. Repeat the same process for that subtree.
7. Go back upward when subtree ends.
8. Continue until all nodes are visited.

## Program:
```
void inorder(node* root)
{
    if (root == NULL)
        return;
    inorder(root->l);
    cout<<"Data="<<root->d<<" "<<"Color="<<root->c<<endl;
    inorder(root->r);
}
```


## Output:
<img width="1146" height="847" alt="Screenshot 2025-11-16 103518" src="https://github.com/user-attachments/assets/ee6324f8-bd75-44e8-9d48-4579d8037d2f" />

##  Result:
Thus the program created successfully for Traversal module of the red black tree in CPP. 

