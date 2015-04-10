# jurnal1

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

package fibonaci;

import java.util.Scanner;

public class Fibonaci {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        int n, i, fibo, tmpfibo;
        tmpfibo = 0;
        Scanner input = new Scanner(System.in);
        System.out.println(" fibonaci ");
        System.out.print("input angka bos = ");
        n = input.nextInt();

        for (i = 0; i <= n; i++) {

            fibo = fibonaci(i);
            System.out.print(fibo + ", ");
            tmpfibo = tmpfibo + fibo;
        }

        System.out.println("total = "+tmpfibo);
    }

    public static int fibonaci(int n) {
        int x;
        if (n == 0) {
            return 0;
        }
        if (n == 1) {
            return (1);
        } else {
            x = fibonaci(n - 1) + fibonaci(n - 2);
        }
        return x;
    }

}
