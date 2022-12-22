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


#another way to print list

//import java.util.LinkedList;
public class MyClass {
    Node head;
    
    class Node 
    {
        int data;
		Node next;

		Node(int d)
		{
			data = d;
			next = null;
		}
	}
	
	public void push(int new_data)
	{
	    Node new_node = new Node(new_data);
	    new_node.next = head;
	    head = new_node;
	}
	
	public void display()
	{
	    Node temp = head;
		while (temp != null) 
		{
			System.out.print(head.data + " ");
			temp = temp.next;
		}
		//System.out.print(temp.data+" ");
	}
	
	public static void main(String[] args)
	{
	    MyClass list = new MyClass();
		
		list.push(24);
		list.push(26);
		System.out.println(" ");
		list.display();
		//list.head = new Node(85);
		//list.head.next = new Node(15);
		//list.head.next.next = new Node(4);
		//list.head.next.next.next = new Node(20);
		//System.out.print(list+" ");
	}
}

