#include <stdio.h>

int main() {
    int choice, quantity;
    float price, total = 0;

    printf("====================================\n");
    printf("       D-MART SUPERMARKET\n");
    printf("====================================\n");

    printf("\nAvailable Products:\n");
    printf("1. Rice        - Rs. 60/kg\n");
    printf("2. Milk        - Rs. 60/litre\n");
    printf("3. Sugar       - Rs. 45/kg\n");
    printf("4. Biscuits    - Rs. 30/packet\n");
    printf("5. Soap        - Rs. 40/piece\n");
    printf("6. Shampoo     - Rs. 120/bottle\n");

    printf("\nEnter product number (1-6): ");
    scanf("%d", &choice);

    switch(choice) {
        case 1:
            price = 60;
            printf("Selected: Rice\n");
            break;

        case 2:
            price = 60;
            printf("Selected: Milk\n");
            break;

        case 3:
            price = 45;
            printf("Selected: Sugar\n");
            break;

        case 4:
            price = 30;
            printf("Selected: Biscuits\n");
            break;

        case 5:
            price = 40;
            printf("Selected: Soap\n");
            break;

        case 6:
            price = 120;
            printf("Selected: Shampoo\n");
            break;

        default:
            printf("Invalid product choice!\n");
            return 0;
    }

    printf("Enter quantity: ");
    scanf("%d", &quantity);

    total = price * quantity;

    printf("\n====================================\n");
    printf("             BILL\n");
    printf("====================================\n");
    printf("Price       : Rs. %.2f\n", price);
    printf("Quantity    : %d\n", quantity);
    printf("Total       : Rs. %.2f\n", total);
    printf("====================================\n");
    printf("Thank you for shopping!\n");

    return 0;
}
