## Ex.No:3

## Ex.Name: Write the right rotate module of splay tree in CPP.

## Aim:
To write the right rotate module of splay tree in CPP.

## Algorithm:
1. Start from the node x to rotate.
2. Let y = x → left (left child of x).
3. Set x → left = y → right.
4. If y → right is not NULL, set y → right → parent = x.
5. Set y → parent = x → parent.
6. If x is root, set root = y.
7. Else if x is left child, set x → parent → left = y.
8. Else, set x → parent → right = y.
9. Set y → right = x.
10. Set x → parent = y.
    
## Program:
```
node *rightRotate(struct node *x)
{
    node *y = x->left;
    x->left = y->right;
    y->right = x;
    return y;
}
```


## Output:
<img width="1195" height="607" alt="Screenshot 2025-11-16 104127" src="https://github.com/user-attachments/assets/93917762-a9e5-43d7-b1e1-aead63db1986" />

## Result:
Thus the program created successfully to right rotate module of splay tree in CPP.


