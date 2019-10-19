# EsempioCalcoloJava
Calcolo del perimetro/area in codifica Java


package esempiocalcolojavatps;

import java.util.Scanner;

/*
 *
 * @author claudio.caputo
 */
 
public class EsempioCalcoloJavaTPS {

    public static void main(String[] args) {
        int b, h, area, perimetro;
        Scanner tastiera = new Scanner(System.in);

        System.out.print("Inserisvi la base");
        b = tastiera.nextInt();
        System.out.print("Inserisci l'altezza");
        h = tastiera.nextInt();

        System.out.println("Area: " + calcolo(b, h, 'a'));
        System.out.println("Perimetro: " + calcolo(b, h, 'p'));
    }

    public static int calcolo(int b, int h, char c) {
        switch (c) {
            case 'p':
                return 2 + (b + h);
            case 'a':
            default:
                return 0;
        }
    }

}

