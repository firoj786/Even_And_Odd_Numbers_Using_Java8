# Even_And_Odd_Numbers_Using_Java8

package Com.nt.practice;

import java.util.Arrays;

/**

 * Creates an array of integers and uses java8 stream API to filter even odd
 
 * numbers into separate arrays. the filter() method is used to keep only even
 
 * or odd numbers,and the- toArray() method is used to convert the resulting
 
 * stream back into an array.
 * 
 * @author 2232829
 *
 */
 
public class EvenAndOddNumberUsingJava8 {

	public static void main(String[] args) {
  
		int arr[] = { 3, 2, 5, 6, 8, 1, 10, 23, 22 };
    
		int evenNumbers[] = Arrays.stream(arr).filter(n -> n % 2 == 0).toArray();
    
		int oddNumbers[] = Arrays.stream(arr).filter(n -> n % 2 != 0).toArray();

		System.out.println("Even Numbers->" + Arrays.toString(evenNumbers));
    
		System.out.println("Odd Numbers->" + Arrays.toString(oddNumbers));

	}

}

Output:-

Even Numbers->[2, 6, 8, 10, 22]
Odd Numbers->[3, 5, 1, 23]

