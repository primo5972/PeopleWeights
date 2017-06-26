# PeopleWeights
School Lab

import java.util.Scanner;
public class PeopleWeights {
public static void main(String[] args) {
double weights[]=new double[5];
Scanner s=new Scanner(System.in);
double sum=0,maxWeight;
for(int i=0;i<5;i++){
System.out.print("Enter weight "+(i+1)+": ");
weights[i]=s.nextDouble();
}
maxWeight=weights[0];
for(int i=0;i<5;i++){
System.out.print("You entered: "+weights[i]+" ");
sum=sum+weights[i];
if(weights[i]>maxWeight){
maxWeight=weights[i];
}
}
System.out.print("\n");
System.out.println("Total weight: "+sum);
System.out.println("Average weight: "+sum/5);
System.out.println("Max weight: "+maxWeight);
}
}
