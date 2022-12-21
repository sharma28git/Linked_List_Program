# LinkedList Program

#Program
Insertion In LinkedList

import java.util.LinkedList;
public class MyClass {
    Node head;    // head of the list
    
    class Node{
        int data;
        Node next;
        
        //constructor to create a new node
        Node(int d){
            data=d;
            next=null;
        }
    }
    
    public void push(int new_data){
        Node new_node = new Node(new_data);
        new_node.next=head;
        head=new_node;
    }
    public static void main(String args[]) {
        LinkedList li = new LinkedList();
        li.push(2);
        li.push(3);
        li.push(4);
        System.out.print(li+" ");
    }
}
