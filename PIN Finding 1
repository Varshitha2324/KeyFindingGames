public class FindPIN {
    public static void main(String[] args) {
        int input1 = 3521;//sample inputs
        int input2 = 2452;//sample inputs
        int input3 = 1352;//sample inputs
        int input4 = 38;//sample inputs

        int pin = findPIN(input1, input2, input3, input4);
        System.out.println("The PIN is: " + pin);
    }

    public static int findPIN(int input1, int input2, int input3, int input4) {
        int largestDigit1 = findLargestDigit(input1);
        int largestDigit2 = findLargestDigit(input2);
        int largestDigit3 = findLargestDigit(input3);

        int pin = (largestDigit1 * largestDigit2 * largestDigit3) + input4;
        return pin;
    }

    private static int findLargestDigit(int number) {
        int largestDigit = 0;
        while (number > 0) {
            int digit = number % 10;
            if (digit > largestDigit) {
                largestDigit = digit;
            }
            number /= 10;
        }
        return largestDigit;
    }
}
