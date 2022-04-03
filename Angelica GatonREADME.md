//*Program 1: Conversation from binary to decimal representation

// Programer:Angelica L. Gaton

//Class: IS 121 Instructor:

  //Pledge: I have neither given nor received unauthorized

  //aid on this program.(Angelica G.)

//Discription: This program converts a binary number to decimal

//Input: Binary Number

//Output: Decimal number//

  

import javax.swing.*;

public class Binary{

  

  public static void main(String[]args)

  {

    String binaryString=JOptionPane.showInputDialog("011011");

    

        int binary=Integer.parseInt(binaryString);

        

        int decimal=0;

        int bit;

        

        int i=0;

        int power2=1;

        int len=binaryString.length();

        

        while(i<len)

        {

          bit=binary%10;

          decimal=decimal+bit*power2;

          

          binary=binary/10;

          power2*=2;

            i++;

        }

        String binaryOutput="Binary:" + binaryString;

        String decimalOutput="Decimal:" + decimal;

        

        JOptionPane.showMessageDialog(null,binaryOutput+"In"+ decimalOutput, "Binary to Decimal Conversion", JOptionPane.INFORMATION_MESSAGE);

        

        

             System.exit(0);

  }

  }
  
  
  
  1. 16 bits- 1111111111111111
  2. 65535
