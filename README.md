package com.company;

import java.util.*;

public class rrr {
    public static void main(String[] args) {
        int n;

        double p1Percent = 0;
        double p2Percent = 0;
        double p3Percent = 0;
        double p4Percent = 0;
        double p5Percent = 0;

        int cntP1 = 0;
        int cntP2 = 0;
        int cntP3 = 0;
        int cntP4 = 0;
        int cntP5 = 0;

        Scanner scr = new Scanner(System.in);

        n =Integer.parseInt(scr.nextLine());

for (int i =0; i < n;i++){
    int currentNumber = Integer.parseInt(scr.nextLine());

    if(currentNumber < 200){
        cntP1++;
    }else if(currentNumber >= 200 && currentNumber <= 399){
        cntP2++;
    }else if(currentNumber >= 400 && currentNumber <= 599){
        cntP3++;
    }else if(currentNumber >= 600 && currentNumber <= 799){
        cntP4++;
    }else{
        cntP5++;
    }
}
        p1Percent =cntP1 * 100 / n;
        p2Percent =cntP2 * 100 / n;
        p3Percent =cntP3 * 100 / n;
        p4Percent =cntP4 * 100 / n;
        p5Percent =cntP5 * 100 / n;

        p1Percent =cntP1 * 100.0 / n;
        p2Percent =cntP2 * 100.0 / n;
        p3Percent =cntP3 * 100.0 / n;
        p4Percent =cntP4 * 100.0 / n;
        p5Percent =cntP5 * 100.0 / n;


        System.out.println(String.format("%.2f%%", p1Percent));
        System.out.println(String.format("%.2f%%", p2Percent));
        System.out.println(String.format("%.2f%%", p3Percent));
        System.out.println(String.format("%.2f%%", p4Percent));
        System.out.println(String.format("%.2f%%", p5Percent));
    }


}
