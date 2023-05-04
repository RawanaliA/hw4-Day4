# hw4-Day4
import java.lang.reflect.Array;
import java.util.ArrayList;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int[] f1 = {50, -20, 0, 30, 40, 60, 10};
        for (int ex : f1)
            if (ex.length[0] == ex.length - 1) {

                System.out.println("it is same yay!");
            } else {
                System.out.println("soray it is Not");
            }
        //solve 2
        int largest[] = {1, 4, 17, 7, 25, 3, 100};
        for (int i = 0; i <= largest.length - 1; i++) {
            System.out.printf("the largest num is:" +Math.Max(i));


        }
        //solve 3اول شي اطلع الافرج بعدها اقارن نتيجه الافرج بكل الارقام الرقم الاكبر المعطى اطبعه لي
        int avrg[] = {1, 4, 17, 7, 25, 3, 100};
        for (int all : avrg) {
            int sum = all + sum / avrg.length - 1;
            if (sum <= all.length - 1) {
                System.out.printf("");
            }
        }
        //solve 4
        int last[] = {20, 30, 40};
        for (int same : last) {
            if (same.lenght(0) >= same.lenght - 1) {
                System.out.printf("the first one is bigger"+same);

            } else {
                System.out.println("the last one is bigger");
            }
        }
        //  for(int i=0;i<= last.length;i++){}

        //number 5هنا انا رجعت الانديكس مو قيمته لازم القيمه
        int swap1[] = {20, 30, 40};
        // System.out.printf("swap ruselt",swap1.length);
        int temp1 = swap1[0];
        temp1 = swap1.length - 1;
        System.out.printf("swap rusle" + temp1);

    }

    //solve 6المعطى سترينق ويبي اطبع اطول الكلمات
    String longest1[] = {"cat", "dog", "red", "is", "am"};
    ArrayList<String> list = new ArrayList<String>();
    int longest_length = 0;
        for (String str : longest1) {
        int length = str.length();
        if (length > longest_length) {
            longest_length = length;
            list.clear();
        }
        if (length == longest_length) {
            list.add(str);
        }
        System.out.println("Original dictionary : "+longest1.toString(longest1));
        System.out.println("Longest word(s) of the above dictionary: "+longest1);
    }


    //solve7
    Scanner s = new Scanner(System.in);
    // Take the array size from the user
        System.out.println("Enter the size of the array: ");
    int arr_size = 0;
        if (s.hasNextInt()) {
        arr_size = s.nextInt();
    }
    // Initialize the array's
    // size using user input
    int[] arr = new int[arr_size];
    // Take user elements for the array
        System.out.println("Enter the elements of the array: ");
        for (int i = 0; i < arr_size; i++) {
        if (s.hasNextInt()) {
            arr[i] = s.nextInt();
        }

        System.out.println(
                "The elements of the array are: ");
        for (int i = 0; i < arr_size; i++) {
            // prints the elements of an array
            System.out.print(arr[i] + " ");
        }
        s.close();
        mainLoop:
        while (true) {
            Scanner inn = new Scanner(System.in);
            System.out.println("\n***Menu***");
            System.out.println("1. Accept elements of an array");
            System.out.println("2. Display elements of an array");
            System.out.println("3. Search the element within array");
            System.out.println("4. Search the element within array");
            System.out.println("5. Sort the array");
            System.out.println("6. To stop");
            System.out.println("Enter action number (1-6): ");

            int command;
            if (inn.hasNextInt()) {
                command = inn.nextInt();
                inn.nextLine();
            } else {
                System.out.println("\nILLEGAL RESPONSE. YOU MUST ENTER A NUMBER.");
                inn.nextLine();
                continue;
            }
            switch (command) {
                case 1:
                    System.out.println("the array elements:" + arr[i]);
            }
        }
        break;
        case 2:
            System.out.println("Original array: ");
            for (int i = 0; i < arr.length; i++) {
                System.out.print(arr[i] + " ");
            }
            break;
        case 3:
            System.out.println("Enter int: ");
            for (int l = 0; l < arr_size; i++) {
                if (s.hasNextInt() == l.) {
                    arr[i] = s.nextInt();
                }
                case 4:
                    int max = arr[0];
                    for (int i = 0; i < arr.length; i++) {
                        if (arr[i] > max)
                            max = arr[i];
                    }
                    System.out.println("Largest element present in given array: " + max);
                    break;
                case 5:
                    for (int m = 0; i < arr_size; i++) {
                        if (m != arr_size)
                            break; // breaks out of the for loop
                    }
                case 6:
                    System.out.println("Stop program");
                    break mainLoop;
                default:
                    System.out.println("Wrong choice!!");

            }
    }
        //solve 8 اعطي ارقام مكرره بالاري ويحسب لي كل رقم كم تكرر مره
    int rep[] = {1, 1, 1, 2, 2, 3};
    int res = 0;int n;
    int x=2;
        for (int i=0; i<n; i++)
        if (x == arr[i])
           int n = arr.length;
         System.out.println(""+arr, n, x));
        }

       }
       //Solve num 9
               int[] arr = { 1, 3, 2, 4,5 };
               // Stores length of array
               int n = arr.length;

               // Traverse array
               for (int i = 0; i < n; i++) {

        for (int j = i + 1; j < n; j++) {

        // If current element is odd
        if (arr[i] >= 1
        && arr[j] >= 1
        && arr[i] % 2 == 1
        && arr[j] % 2 != 1) {

        // Perform Swap
        int tmp = arr[i];
        arr[i] = arr[j];
        arr[j] = tmp;

        // Change the sign
        arr[j] = -arr[j];

        break;
        }

        // If current element is odd
        // then swap it with even
        else if (arr[i] >= 1
        && arr[j] >= 1
        && arr[i] % 2 != 1
        && arr[j] % 2 == 1) {

        // Perform Swap
        int tmp = arr[i];
        arr[i] = arr[j];
        arr[j] = tmp;

        // Change the sign
        arr[j] = -arr[j];

        break;
       }

        }}
               //Solve num 10
        int arr4[] = { 2,3,6,6,4 };
        int arr5[] = { 2,3,6,6,4 };
        for(int i=0;i<=arr4.length;i++){
        for (int j=0;j<=arr5.length;i++){
        if(i==j) {
        System.out.println("it is Equel");
        break;
        }
        }
