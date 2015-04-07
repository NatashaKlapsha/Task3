# Task3
package Qsort;

/**
 * Created by Natalia on 04.04.2015.
 */
public class ShiftSort implements Sorting{
    @Override
    public void sort(int[] array) {
        for (int i = 0; i <array.length; i++)
        {
            int temp = array[i];
            int j =i-1;
            while(j >= 0 && array[j] > temp)
            {
                array[j + 1] = array[j];
                j--;
            }
            array[j + 1] = temp;
        }

    }
}
