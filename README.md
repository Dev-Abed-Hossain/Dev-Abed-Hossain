<?php
// 1st assignment: একজন ইউজারের বিয়ের সঠিক বয়স বের করার জন্য একটি প্রোগ্রাম লিখুন যেখানে একজন ইউজার ওনার নাম, জন্মসালে এবং জেন্ডার দিয়ে চেক করবেন। 

echo "1. </br>";

$name = "Lamia";
$birth_year = 2001;
$gender = "Female";

$age = 2024 - $birth_year;
$wait = 21 - $age;


if($gender == "Male"){
    if($age >= 21){
        echo "Hello {$name} brother, You are ready to get married.";
    }else{
        echo "Hello {$name} brother, You can not get married yet. You have to wait {$wait} years to get married.";
    }
}else if($gender == "Female" ) {
    if($age >= 18){
        echo "Hello {$name} sister, You are ready to get married.";
    }else{
        echo "Hello {$name} sister, You can not get married yet. You have to wait {$wait} years to get married.";
    }
}else{
    echo "Hello {$name}, Please put the valid data.";
}

echo "</br>";
echo "</br>";



// 2nd assignment: একটি কারেন্সি কনভার্টার এপলিকেসন বানান যেখানে আমরা ডলার, পাওন্ড, ইউরো  কে টাকায় দেখতে পারবো  

echo "2. </br>";

$amount = 50;
$currency = "Found";

switch ($currency) {
    case 'Dollar':
        echo "{$amount} {$currency} convert it bangladesh taka equal " . $amount * 120 . " taka";
        break;
    case 'Found':
        echo "{$amount} {$currency} convert it bangladesh taka equal " . $amount * 150 . " taka";
        break;
    case 'Euro':
        echo "{$amount} {$currency} convert it bangladesh taka equal " . $amount * 133 . " taka";
        break;
    default:
        echo "Please put the right currency.";
        break;
}


echo "</br>";
echo "</br>";

// 3rd assignment: একটি ত্রিভুজ, আয়তক্ষেত্র, বর্গক্ষেত্র এবং বৃত্তের ক্ষেত্রফল বের করার জন্য প্রোগ্রাম লিখুন  

echo "3. </br>";

$x_access = 10;
$y_access = 20;
$type = "Triangle";

if($type == "Triangle"){
    echo "{$type} area = " . .5 * $x_access * $y_access;
}else if($type == "Ractangle"){
    echo "{$type} are = " . $x_access * $y_access; 
}else if($type == "Square"){
    echo "{$type} are = " . $x_access * $x_access;
}else if($type == "Circle"){
    echo "{$type} are = " . 3.1416 * $x_access * $x_access;
}else{
    echo "Please input valid data.";
}

echo "</br>";
echo "</br>";

// 4th assignment: BMI বের করার জন্য একটি এপ্লিকেসন বানান যেখানে যে কেউ তার BMI বের করতে পারবে

echo "4. </br>";

$$name = "Abed Hossain";
$$age = 28;
$height = 5.7;
$wight = 74;

$height_m = $height / 3.2808;

$bmi = $wight / ($height_m * 2);

$bmi_two = number_format($bmi, 1);

if($bmi < 18.5){
    echo "Hello {$$name}, Your BMI is {$bmi_two} under weight. You have to gain a lot weight.";
}else if($bmi >= 18.5 && $bmi <= 24.9){
    echo "Hello {$$name}, Your BMI is {$bmi_two} normal. You have to maintain this weight.";
}else if($bmi >= 25 && $bmi <= 29.9){
    echo "Hello {$$name}, Your BMI is {$bmi_two} over weight. You have to lose weight.";
}else if($bmi >= 30){
    echo "Hello {$$name}, Your BMI is {$bmi_two} obesity. You have to lose weight as well as mantain strong dude.";
}else{
    echo "Please put valid data.";
}


echo "</br>";
echo "</br>";

// 5th assignment: একটি গ্রেডিং এপলিকেসন বানান যেখানে কেউ কোন সাবজেক্ট এর মার্ক দিলে সেটা আপনাকে Grade and GPA  বলে দিবে 

echo "5. </br>";

$$$name = "Abed Hossain";
$class = "Seven";
$roll = 12;
$bangla = 78;

if($bangla >= 0 && $bangla < 33){
    echo "Hello {$$$name}
    </br>
    Marks   :   {$bangla}
    </br>
    Grade   :   F
    </br>
    GPA :   0";
}else if($bangla >= 33 && $bangla < 40){
    echo "Hello {$$$name}
    </br>
    Marks   :   {$bangla}
    </br>
    Grade   :   D
    </br>
    GPA :   1";
}else if($bangla >= 40 && $bangla < 50){
    echo "Hello {$$$name}
    </br>
    Marks   :   {$bangla}
    </br>
    Grade   :   C
    </br>
    GPA :   2";
}else if($bangla >= 50 && $bangla < 60){
    echo "Hello {$$$name}
    </br>
    Marks   :   {$bangla}
    </br>
    Grade   :   B
    </br>
    GPA :   3";
}else if($bangla >= 60 && $bangla < 70){
    echo "Hello {$$$name}
    </br>
    Marks   :   {$bangla}
    </br>
    Grade   :   A-
    </br>
    GPA :   3.5";
}else if($bangla >= 70 && $bangla < 80){
    echo "Hello {$$$name}
    </br>
    Marks   :   {$bangla}
    </br>
    Grade   :   A
    </br>
    GPA :   4";
}else if($bangla >= 80 && $bangla <= 100){
    echo "Hello {$$$name}
    </br>
    Marks   :   {$bangla}
    </br>
    Grade   :   A+
    </br>
    GPA :   5";
}else{
    echo "Please input valid data.";
}


?>
