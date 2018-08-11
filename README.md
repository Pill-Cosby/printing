# printing
public static void printStars(int size) {
        int i = 1;
        while (i <= size) {
            System.out.print("*");
            i++;
        }
        System.out.println("");
    }

    public static void printRectangle(int width, int height) {
        int count = 1;
        while (count <= height) {
            printStars(width);
            count++;
        }
    }

    public static void printWhiteSpaces(int size) {
        int i = 1;
        while (i <= size) {
            System.out.print(" ");
            i++;
        }
    }

    public static void printTriangle(int size) {
        int i = 1;
        while (i <= size) {
            printWhiteSpaces(size - i);
            printStars(i);
            i++;
        }
    }

    public static void xmasTree(int height) {
        int i = 1;
        while (i <= height) {
            printWhiteSpaces(height - i);
            printStars(i + (i - 1));
            i++;
        }
        printWhiteSpaces(height - 2);
        printStars(3);
        printWhiteSpaces(height - 2);
        printStars(3);
    }

    public static void main(String[] args) {

        printTriangle(4);
        System.out.println("---");
        xmasTree(4);
        System.out.println("---");
        xmasTree(10);
    }
}
