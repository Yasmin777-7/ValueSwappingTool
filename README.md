# Value Swapping Tool | Değişken Değiştirme Aracı 🔄

### Description | Açıklama:
**EN:** This project explains the logic of swapping two numerical values using a third temporary variable. It is a fundamental concept in logic and software engineering.
**TR:** Bu proje, üçüncü bir geçici değişken kullanarak iki sayısal değerin yerini değiştirme mantığını açıklamaktadır. Mantık ve yazılım mühendisliğinde temel bir kavramdır.

---

## 📊 Flowchart | Akış Diyagramı
**EN:** The following diagram shows the step-by-step process of the swapping algorithm:  
**TR:** Aşağıdaki diyagram, değiştirme algoritmasının adım adım sürecini göstermektedir:

![Flowchart](ValueSwappingFlowchart.png)

---

## 🧠 Logic Steps | Mantık Adımları:

### 1. Initial State (Before Swapping) | İlk Durum:
- **Num1:** Value A
- **Num2:** Value B
- **Temp:** Empty | Boş

### 2. The Swap Process | Değiştirme İşlemi:
1. **Move Num1 to Temp:** Safe storage of the first value.
2. **Move Num2 to Num1:** The first variable now holds the second value.
3. **Move Temp to Num2:** The second variable now holds the stored first value.

### 3. Final State (After Swapping) | Son Durum:
- **Num1:** Value B
- **Num2:** Value A

  

import java.util.Scanner;
public class Main {
    public static void main(String[] args){
    Scanner s1 = new Scanner(System.in) ;

        System.out.println("Enter your num1:");
    int num1 = s1.nextInt();
        System.out.println("Enter your num2:");
    int num2 = s1.nextInt();

        System.out.println("___Before Swapping___");
        System.out.println(num1);
        System.out.println(num2);

        int temp = num1;
        num1 = num2;
        num2 =  temp;

        System.out.println("___After Swapping___");
        System.out.println(num1);
        System.out.println(num2);
    }
}

