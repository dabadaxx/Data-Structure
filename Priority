package GroceryDistribution;

public class Priority {

private GroceryItem[] items;

private int current;

public Priority(int size)

{

	items = new GroceryItem[size];

current = 0;

	}
	
	public void insert(GroceryItem s)
	
	{
	
	if(!isFull())
	
	{
	
	//find the correct place where to insert new 
	
	int insertPoint = 0;
	
	while(insertPoint < current)
	
	{
	
	if(s.getItemWeight() <= items[insertPoint].getItemWeight())
	
	insertPoint++;
	
	else
	
	break;
	
	}
	
	//since we want to insert at insertPoint, move all elements starting from
	
	//insertPoint to end , one position right
	
	for(int i = current - 1; i >= insertPoint; i--)
	
		items[i+1] = items[i];
	
	//now insert the new state
	
	items[insertPoint] = s;
	
	current++;
	
	}
	
	}
	
	public GroceryItem remove()
	
	{
	
		GroceryItem val = null;
	
	if(!isEmpty())
	
	{
	
	val = items[0]; //get the 1st element
	
	//move all others one place left
	
	for(int i = 1; i < current; i++)
	
		items[i-1] = items[i];
	
	current--;
	
	}
	
	return val;
	
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
	
	public void printQueue()
	
	{
		System.out.println("");

		Double sum = 0.00;
		
		// GroceryItem name ;
		// System.out.println("============== Truck with" + items.length + " items going from BC Warehouse to "+ items[3].getDestination() + "=============");
		for(int i = 0; i < current; i++)
		{
		//  System.out.println(items[i]);
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


