class Main {
    public static void main(String[] args) {
        System.out.println("hello ji");
    }
}
//hii
class Example{
    public static void main(String[] args){
        System.out.println("hiiii");
        
        //statically typed language
//can't change
boolean num =true;
String course="python";
int score=56;
// String score="56"; error
float marks= 7.8f;

// operator all same as python but not **
// Number num=2**3
if(score>0){
    System.out.println("positive");
}
int[] number={1,2,3,4,7,8,9};
for(int a:number){
    if(a==8){
        break;
    }
    if(a==2 || a==3){
        continue;
    }
    
     System.out.println(a);
}
    }
}

// py   java
// and   &&
// or     ||
// not    !

//elif    else if

//for  in :        for (type a: num){}


////

//premitive
//double num=4.5
// float num2=6.7s
//char grade='A' //"A" err

//non-premitive
//1//String name="sapna" //'sapan' err
//2//arr int[] num={1,2,3,4,5}
// int[] num= new int[]
// num[0]=24
//3//class pascal case class MyName{}
//

import java.util.*;
//date and time 
import java.time.LocalDate;
import java.time.LocalTime;
// from datetime import datetime;
import java.time.Period;
// import java.time.LocalDate;
import java.time.Duration;
import java.time.LocalTime;
import java.time.format.DateTimeFormatter;

class Rectangle{
    int h;
    int w;
    Rectangle(int h, int w){
        this.h=h;
        this.w=w;
    }
    int get_width(){
        return this.h;
    }
    void get_area(){
        System.out.println(this.h*this.w);
    }
}







class Main {
    public static void main(String[] args) {
        System.out.println("Be the programmer, you're meant to be!");
   
       Rectangle rect= new Rectangle(10,30);
       System.out.println(rect.h);
       System.out.println(rect.get_width());
       rect.get_area();
       //date 
        LocalDate dateObj =LocalDate.of(2019,10,5);
        System.out.println(dateObj);
        System.out.println(dateObj.now());
        
        //
         LocalTime timeObj = LocalTime.of(11, 34, 56);
        System.out.println(timeObj);
         System.out.println(timeObj.getHour());
        System.out.println(timeObj.getMinute());
        System.out.println(timeObj.getSecond());
        
        //
        
        
    //   date_time_obj = datetime(2018, 11, 28, 10, 15, 26);
    //   print(date_time_obj.year);
    //   print(date_time_obj.month);
    //   print(date_time_obj.hour);
    //   print(date_time_obj.minute);
      
      ///
      
       LocalDate startDate = LocalDate.of(2020, 2, 20);
        LocalDate endDate = LocalDate.of(2021, 10, 21);
        Period period = Period.between(startDate, endDate);
        System.out.println("Years: " + period.getYears());
        System.out.println("Months: " + period.getMonths());
        System.out.println("Days: " + period.getDays());
        ///
        
         LocalTime startTime = LocalTime.of(10, 30, 30);
        LocalTime endTime = LocalTime.of(10, 31, 30);
        Duration duration = Duration.between(startTime, endTime);
        System.out.println(duration.getSeconds());
        
        
        ///


        List<Integer> numbers = Arrays.asList(2, 5, 6, 1);

        numbers.stream()
               .sorted((num1, num2) -> num2 - num1) // sorts the numbers in descending order
               .forEach(number -> System.out.println(number));
    

    }
}


//in py
// from datetime import date, datetime

// mydate= date(2000,10,25)
// mydateTime= datetime(2000,10,25,2,34,45)
// print(mydate, mydateTime)