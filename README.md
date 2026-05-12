# ll_insert_at_specific_position
python code for insert at specific position a new node in singly ll

class Node:
    def __init__(self, data):
        self.data = data
        self.next = None




n1=Node(5)
n2=Node(10)
n3=Node(15)


n1.next=n2
n2.next=n3


new_node=Node(25)
head=n1
curr=head
while curr is not None:
    if curr.data==10:
        
        new_node.next=curr.next
        curr.next=new_node
        break
        
       
    curr=curr.next
curr=head
while curr is not None:
    print(curr.data,end=" ")
    if curr.next is not None:
        print("->",end=" ")
    curr=curr.next

