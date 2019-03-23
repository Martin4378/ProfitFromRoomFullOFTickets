# ProfitFromRoomFullOFTickets

import java.util.Scanner;

public class P34_ProfitFromRoomFullOFTickets {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        String ticketType = scanner.nextLine();
        int numberRows = Integer.parseInt(scanner.nextLine());
        int numberColums  = Integer.parseInt(scanner.nextLine());
        double ticketPrice = 0;

        switch (ticketType){

            case "Premiere":
                ticketPrice = 12.00;
                break;

            case "Normal":
                ticketPrice = 7.50;
                break;

            case "Discount":
                ticketPrice = 5.00;
                break;

        }

        double profit = ticketPrice * numberColums * numberRows;

        System.out.printf("%.2f leva\n", profit);


    }

}
