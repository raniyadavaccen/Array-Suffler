# Array-Suffler
To Suffle the given Array using Java programming language

import java.util.ArrayList;
import java.util.Arrays; // Add this import statement
import java.util.Collections;
import java.util.List;

public class ArraySuffler {
    public static void main(String[] args) {
        // Create an array with the values (1, 2, 3, 4, 5, 6, 7)
        Integer[] array = {1, 2, 3, 4, 5, 6, 7};

        // Convert the array to a list for shuffling
        List<Integer> list = new ArrayList<>(Arrays.asList(array));

        // Shuffle the list
        Collections.shuffle(list);

        // Convert the shuffled list back to an array
        Integer[] shuffledArray = list.toArray(new Integer[0]);

        // Print the shuffled array
        for (Integer value : shuffledArray) {
            System.out.print(value + " ");
        }
    }
}
