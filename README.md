# hw4-Day4
import java.util.ArrayList;
import java.util.Arrays;
import java.util.Collections;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        //solve 1
        int[] num_arr1 = {50, -20, 0, 30, 40, 60, 10};
        System.out.println(num_arr1.length >= 2 && num_arr1[0] == num_arr1[num_arr1.length - 1]);

        //solve 2
        Integer number[] = {1, 4, 17, 7, 25, 3, 100};
        int k = 1;
        Arrays.sort(number, Collections.reverseOrder());
        System.out.println(k + " The largest elements of  array are:");
        for (int i = 0; i < k; i++)
            System.out.print(number[i] + " ");
        //solve 3
        int nums[] = {1, 4, 17, 7, 25, 3, 100};
        int sum = 0;
        System.out.println("Original Array: ");
        System.out.println(Arrays.toString(nums));
        for (int i = 0; i < nums.length; i++) {
            sum = sum + nums[i];
        }
        double average = sum / nums.length;
        System.out.println("The average of the said array is: " + average);
        System.out.println("The numbers in the said array that are greater than the average are: ");
        for (int i = 0; i < nums.length; i++) {
            if (nums[i] > average) {
                System.out.println(nums[i]);
            }
            //solve 4
            int[] arr_larger = {20, 30, 40};
            int max_val = arr_larger[0];
            if(arr_larger[2] >= max_val)
                max_val = arr_larger[2];
            System.out.println("Larger value between first and last element: "+max_val);

           //solve 5
            int[] array = {20, 30, 40};
            System.out.println("Original Array: "+Arrays.toString(array));
            int x = array[0];
            array[0] = array[array.length-1];
            array[array.length-1] = x;
            System.out.println("New array after swaping the first and last elements: "+Arrays.toString(array));
           //solve 6
            ArrayList<String> list = new ArrayList<String>();
            String [] dict = {"cat", "dog", "red", "is", "am"};
            System.out.println("Original dictionary : "+ Arrays.toString(dict));
            int longest_length = 0;
            for (String str : dict) {
                int length = str.length();
                if (length > longest_length) {
                    longest_length = length;
                    list.clear();
                }
                if (length == longest_length) {
                    list.add(str);
                }
                System.out.println(""+list);
            }
            //solve 7
            System.out.print("Enter the number of elements you want to store: ");
                Scanner sc = new Scanner(System.in);
                int n = sc.nextInt();
                int[] array2 = new int[n];

                System.out.println("Enter the elements of the array: ");
                for (int d= 0; d < n; d++) {
                    array2[d] = sc.nextInt();
                }

                mainLoop:
                while (true) {
                    Scanner inn = new Scanner(System.in);
                    System.out.println("\n***Menu***");
                    System.out.println("1. Accept element of array");
                    System.out.println("2. Display element of an array");
                    System.out.println("3. Search elements");
                    System.out.println("4. Sort the array in descending way");
                    System.out.println("5. To stop the program");
                    System.out.println("Enter action number (1-5): ");
                    int command;
                    if (inn.hasNextInt()) {
                        command = inn.nextInt();
                        inn.nextLine();
                    } else {
                        System.out.println("\n YOU MUST ENTER A NUMBER.");
                        inn.nextLine();
                        continue;
                    }
                    switch (command) {
                        case 1:
                            System.out.println(": ");
                            for (int d = 0; d < array2.length; d++) {
                                System.out.println(array2[i]);
                            }

                            break;
                        case 2:
                            System.out.println("Array elements are: ");
                            for (int d = 0; d < n; d++) {
                                System.out.println(array2[d]);
                            }
                            break;
                        case 3:
                            boolean found = false;
                            System.out.println("Enter the value you want to search for");
                            int v = sc.nextInt();
                            for (int d = 0; d < array2.length; d++) {
                                if (v == array2[i]) {
                                    found = true;
                                    System.out.println("The number you are search for Is" + v);
                                }
                                if (!found) {
                                    System.out.println("not found");
                                }
                            }
                        case 4:
                            int temp;
                            for (int d = 0; d < array2.length; d++) {
                                for (int j = d+ 1; j < array2.length; j++) {
                                    if (array2[i] > array2[j]) {
                                        temp = array2[d];

                                        temp = array2[d];
                                        array2[d] = array2[j];
                                        array2[j] = temp;}
                                }
                            }
                            System.out.println("Array elements in descending order:");
                            //accessing element of the array
                            for (int d = 0; d <= array2.length - 1; d++) {
                                System.out.println(array2[i]);
                            }
                        case 5:
                            System.out.println("Program terminated");
                            break mainLoop;
                        default:
                            System.out.println("Wrong choice!!");

//solve 8 اتاكد انو يطبع كل الارقام
            int[] arr = {1, 1, 1, 3, 3, 5};
            int Count1 = 0;

            int count = 0;
            for (int j = 0; j < arr.length; j++) {
                if (arr[j] == Count1+1) {
                    count++;
                }
            }
            System.out.println("The element " + Count1 + " appears " + count + " times in the array.");
    }
    //solve 9
        int[] arra= {2,3,40,1,5,9,4,10,7};
        int a = 0;
        System.out.println("Original Array: "+Arrays.toString(arra));
        while(a < arra.length && arra[a] % 2 == 0)
            a++;
        for(int j = a + 1; j < arra.length; j++) {
            if(arra[j] % 2 != 0) {
                int temp = arra[a];
                arra[a] = arra[j];
                arra[j] = temp;
                a++;}}
        System.out.println("New Array: "+Arrays.toString(arra));
        //solve 10
        int [] arr1 = new int [] {20, 5, -95, 43, 17};
        int [] arr2 = new int [] {20, 5, -95, 43, 17};
        System.out.println(Arrays.equals(arr1, arr2));
    }}
    }}
