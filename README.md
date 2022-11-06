- 👋 Hi, I’m @ah2025
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
ah2025/ah2025 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import java.util.Scanner;
public class BMI {

    public static void main(String[] args) throws Exception {
        calculateBMI();
        
    }
   
    private static void calculateBMI() throws Exception {
        
        Scanner s = new Scanner(System.in);
        
        System.out.print("Please enter your weight in kg: \n");
        
        float weight = s.nextFloat();
        System.out.print("Please enter your height in cm: \n");
        float height = s.nextFloat();
         
       
        float bmi = (100*100*weight)/(height*height);
         System.out.println("Hello Nini");
        System.out.println("Your BMI is: "+bmi);
        printBMICategory(bmi);
         
    }
     
    private static void printBMICategory(float bmi)
    
    
    
    {
        if(bmi < 18.5) {
            System.out.println("You are underweight");
        }else if (bmi < 24.9) {
            System.out.println("You are normal");
        }else if (bmi < 29.9) {
            System.out.println("You are overweight");
        }else {
            System.out.println("You are Very Overweight");
        }
    }
} 
    
