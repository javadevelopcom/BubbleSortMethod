# BubbleSortMethod
Bubble Sort Method
public class BubbleSortMethod {
    public static void main(String[] args) {
        int[] num = new int[5];
        num[0] = 44;
        num[1] = 1;
        num[2] = 20;
        num[3] = 5;
        num[4] = 10;

        System.out.println("Unsorted array:");
        for (int i : num) {
            System.out.println(i);
        }
        for (int a = 1; a < num.length; a++)
            for (int b = num.length - 1; b >= a; b--) {
                if (num[b - 1] > num[b]) {
                    int z = num[b - 1];
                    num[b - 1] = num[b];
                    num[b] = z;
                }
            }
        System.out.println("Sorted array:");
        for (int i = 0; i < num.length; i++)
            System.out.println(num[i]);
    }
}
