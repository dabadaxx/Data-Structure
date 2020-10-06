package GroceryDistribution;

import java.util.Arrays;

public class Stack {
	
	private GroceryItem[] items;

	private int current;

	public Stack(int size)

	{

		items = new GroceryItem[size];

	current = 0;

	}

	public void push(GroceryItem s)

	{

	if(!isFull())

		items[current++] = s;

	}

	public GroceryItem pop()

	{

	if(!isEmpty())

	return items[--current];

	else

	return null;

	}

	public boolean isEmpty()

	{

	return current == 0;

	}

	public boolean isFull()

	{

	return current == items.length;

	}

	public int size()

	{

	return current;

	}

	public void printStack()

	{

	System.out.println("");

	Double sum = 0.00;
	
	// GroceryItem name ;
	// System.out.println("============== Truck with" + items.length + " items going from " + items[3].getDestination() +"to BC Warehouse=============");
	for(int i = current - 1; i >= 0; i--)
	{
	// System.out.println(items[i]);
	System.out.println("GroceryItem [itemName= " + items[0] 
    		+ "," + " itemWeight= " + items[1]
    				+ ", destination= " + 
    				items[2] + "," + " origin= "
    				+ items[3] + "]");
	sum+=items[1].getItemWeight();

	}
	System.out.println("=== Truck Weight" + sum + "  kilograms =================================");
	}
}
	

