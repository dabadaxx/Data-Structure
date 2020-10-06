package GroceryDistribution;

import java.io.*;
import java.util.Scanner;
import java.util.Stack;

import QueuePackage.*;
import StackPackage.StackInterface;

/**
 * 
 * @author YOUR NAME HERE
 *
 */
public class SendStockToStores {
	public static void main(String[] args) throws NumberFormatException, IOException {

		String fileName = "GroceryItems.csv";
		Scanner textReader = null;
		String line = "";
		Stack stack = new Stack();

		// your code here
		try {
			
		

			BufferedReader br = new BufferedReader(new FileReader(fileName));
			// to ignore the first line
			
			
			while ((line = br.readLine()) != null) {
				
				System.out.println("################ Unloading trucks at warehouse\r\n" + 
						"\r\n" + 
						"################ Displaying warehouse with 74 items");
            while ((line = br.readLine()) != null) {
				System.out.println("################\r\n" + 
						"\r\n" + 
						"=============== Displaying contents of loaded trucks travelling from warehouse to destination");
            while ((line = br.readLine()) != null) {

                String[] data = line.split(",");
// we have 4 column
                if(data != null && data.length == 4){

                    // Only state from region South, West or Midwest
                   // if("Toronto".equals(data[4]) || "Calary".equals(data[4]) ||
                  //  		"Califoria".equals(data[4])){
                        GroceryItem items = new GroceryItem(data[0], 
                        		Double.parseDouble(data[1]), data[2],
                                (data[3]));

                        // Pushing state to stack
                      //  stack.push(state);
                        System.out.println("GroceryItem [itemName= " + data[0] 
                        		+ "," + " itemWeight= " + data[1]
                        				+ ", destination= " + 
                        				data[2] + "," + " origin= " 
                        				+ data[3] + "]");
                        stack.push(items);


                    }
             //   inFile.close();
               
                }
            
            
            }
            stack.printStack();
	}}
		catch (FileNotFoundException e) {
			
		}

}
	
	static <T> void displayQueue(QueueInterface<T> queue) {
        Object[] items = queue.toArray();
        System.out.println("============== Truck with" + items.length + "items going from" + " " + "to BC Warehouse=============");
        if (items != null) {
            System.out.println("GroceryItem [itemName= " + items[0] + "," + " itemWeight= " + items[1] + ", destination= " + items[2] + "," + " origin= " + items[3] + "]");
            Object[] var5 = items;
            int var4 = items.length;

            for(int var3 = 0; var3 < var4; ++var3) {
                Object item = var5[var3];
                System.out.print(" " + item);
            }

            System.out.println();
        }
    }

    static <T> void displayStack(StackInterface<T> stack) {
        Object[] stackEntries = stack.toArray();
        displayStack(stackEntries, stack.size());
    }

    static <T> void displayStack(Stack<T> stack) {
        Object[] stackEntries = stack.toArray();
        displayStack(stackEntries, stack.size());
    }

    static <T> void displayStack(T[] stack, int size) {
        System.out.println("============== Truck with" + size + "items going from " + " to BC Warehouse=============");

        for(int index = 0; index < size; ++index) {
            System.out.print(" " + stack[index]);
        }

        System.out.println();
    }
}
