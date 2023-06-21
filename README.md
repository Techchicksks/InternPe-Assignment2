# InternPe-Assignment2
 printed an American flag on the screen.

 
public class AmericanFlag {
    public static void main(String[] args) {
        int width = 60; // Width of the flag in characters
        int height = 30; // Height of the flag in characters

        // Print the top part of the flag
        for (int i = 0; i < height / 2; i++) {
            // Print the red and white stripes
            for (int j = 0; j < width; j++) {
                if (j % 2 == 0) {
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }

        // Print the blue field
        for (int i = 0; i < height / 2; i++) {
            for (int j = 0; j < width; j++) {
                if (j < width / 2 && i < height / 2) {
                    System.out.print(" ");
                } else {
                    System.out.print("#");
                }
            }
            System.out.println();
        }
    }
}
