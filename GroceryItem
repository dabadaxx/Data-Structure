package GroceryDistribution;

/**
 * @author YOUR NAME HERE
 *
 */
public class GroceryItem {

	private String itemName;
	private double itemWeight;
	private String destination;
	private String origin;
	
   
	
	public GroceryItem(String itemName, double itemWeight, String destination, String origin) {
		
		this.itemName = itemName;
		this.itemWeight = itemWeight;
		this.destination = destination;
		this.origin = origin;
	}
	
	public String getItemName() {
		return itemName;
	}
	public double getItemWeight() {
		return itemWeight;
	}
	public String getDestination() {
		return destination;
	}
	public String getOrigin() {
		return origin;
	}
	public void setItemName(String itemName) {
		this.itemName = itemName;
	}
	public void setItemWeight(double itemWeight) {
		this.itemWeight = itemWeight;
	}
	public void setDestination(String destination) {
		this.destination = destination;
	}
	public void setOrigin(String origin) {
		this.origin = origin;
	}
	public int CompareToDestination(GroceryItem destination)
    {
        // your code here
        if (destination != null )
        {
            return destination.CompareToDestination(destination);
        }
        return 0;
    }
	public int CompareToOrigin(GroceryItem origin)
    {
        // your code here
        if (origin != null )
        {
            return origin.CompareToOrigin(origin);
        }
        return 0;
    }
	public int Compare(GroceryItem a, GroceryItem b)
    {
        // your code here

        if (a != null && b != null)
        {
            return a.origin.compareTo(b.origin);
        }

        return 0;

    }
	 @Override
		public String toString() {
			// TODO Auto-generated method stub
		 return "GroceryItem [itemName=" + this.itemName + ", " 
					+ "itemWeight=" + this.itemWeight + ", " 
		 + "destination=" + this.destination + ", " + "origin" 
					+ this.origin + ", " + "]";
	    }
	 public void display() {
	        System.out.println("GroceryItem [itemName= " +
	 this.itemName + "," + " itemWeight= " + this.itemWeight + ","
	 		+ " destination= " + this.destination + "," + " origin= " + this.origin + "]");
	    }
}
	 
