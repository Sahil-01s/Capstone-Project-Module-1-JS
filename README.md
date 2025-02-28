function calculateBMI(weight, height) {
    // Write your code here
    if(weight <=0 || height<=0){
    return "Invalid input: Weight and height must be positive numbers.";
    }
    const bmi =  weight/(height*height);
   
    if (bmi < 18.5) {
        return "Underweight";
    } else if (bmi >= 18.5 && bmi < 24.9) {
        return "Normal weight";
    } else if (bmi >= 25 && bmi < 29.9) {
        return "Overweight";
    } else {
        return "Obese";
    }
}
