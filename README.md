# algorithm-flowchart-workshop
An Algo and flowchart workshop

## 1. Check Even or Odd Number

Design an algorithm and flowchart that take a number as input and determine whether it is **even or odd**.

### ✔ Pseudocode

```text
START
    INPUT number
    IF number % 2 == 0 THEN
        PRINT Even
    ELSE
        PRINT Odd
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Get input N/]
    B --> C{N % 2 == 0 ?}
    C -->|Yes| D[/Print Even/]
    C -->|No| E[/Print Odd/]
    D --> F([End])
    E --> F
```

---

## 2. Calculate Total and Average Marks

Write the algorithm and draw the flowchart for a program that inputs **marks for 3 subjects**, calculates the **total and average**, and displays both.

### ✔ Pseudocode

```text
Start
    INPUT grade1, grade2, grade3
    Total = grade1+grade2+grade3
    Average = Total/3
    DISPLAY "Total is " + Total
    DISPLAY "Average is " + Average
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input grade1, grade2, grade3/]
    B --> C[Total = grade1 + grade2 + grade3]
    C --> D["Average = Total / 3"]
    D --> E[/"Display #quot;Total is #quot; + Total"/]
    E --> F[/"Display #quot;Average is #quot; + Average"/]
    F --> G([End])
```

---

## 3. Display Multiplication Table

Create an algorithm and flowchart that input a number and display its **multiplication table from 1 to 10** using a loop.

### ✔ Pseudocode

```text
Start
Input Number
FOR i = 1 TO 10
Display Number * i
ENDFOR
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input Number/]
    B --> C[i = 0]
    C --> D[i = i + 1]
    D --> E[/Display Number * i/]
    E --> F{"i >= 10"}
    F -->|Yes| G([End])
    F -->|No| D
```

---

## 4. Positive, Negative, or Zero Check

Write the algorithm and flowchart to input a number and display whether it is **positive, negative, or zero**.

### ✔ Pseudocode

```text
START
    INPUT number
    IF Number > 0      
        Display "positive"
    ELSE IF  Number < 0
        Display "negative"
    Else
        Display "zero"
    ENDIF
End
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/INPUT number/]
    B --> C{"number > 0"}
    C -->|Yes| D[/"Print #quot;positive#quot;"/]
    C -->|No| E{"number < 0"}
    D --> F([End])
    E -->|Yes| G[/"Print #quot;negative#quot;"/]
    E -->|No| H[/"Print #quot;zero#quot;"/]
    G --> F
    H --> F
```

---

## 5. Simple Interest Calculator

Create an algorithm and flowchart for a program that calculates simple interest using **SI = (P × R × T) / 100**. P = principal (the original amount), R = rate of interest (percent per year), T = time in years.

### ✔ Pseudocode

```text
START
    INPUT principal, rate, time
        SI = (principal*rate*time) / 100
   PRINT "simple interest = " + SI 
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/INPUT principal, rate, time/]
    B --> C["SI = (principal * rate * time) / 100"]
    C --> D[/"Print #quot;Simple interest = #quot; + SI"/]
    D --> E([End])
```

---

## 6. Average Temperature Calculation

Write the algorithm and draw the flowchart for a program that takes the **temperature of 7 days**, finds the **average temperature**, and displays it.

### ✔ Pseudocode

```text
START
    INPUT day1, day2, day3, day4, day5, day6, day7
    at = (day1 + day2 + day3 + day4 + day5 + day6 + day7) / 7
    PRINT "average temperature = " + at
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input day1, day2, day3, day4, day5, day6, day7/]
    B --> C["at = (day1 + day2 + day3 + day4 + day5 + day6 + day7) / 7"]
    C --> D[/"PRINT #quot;average temperature = #quot; + at"/]
    D --> E([End])
```

---

## 7. Calculate Area of a Rectangle

Create an algorithm and flowchart to input **length and width**, calculate the area (**Area = Length × Width**), and display the result.

### ✔ Pseudocode

```text
START
    INPUT length, width
    area = length * width
    PRINT "area = " + area 
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input length, width/]
    B --> C[area = length * width]
    C --> D[/"Print #quot;area = #quot; + area"/]
    D --> E([End])
```

---

## 8. Determine Pass or Fail

Write the algorithm and draw the flowchart for a program that takes a student's average marks and displays **"Pass"** if average ≥ 50, otherwise **"Fail"**.

### ✔ Pseudocode

```text
START
    INPUT averageMark
    IF  averageMark>=50
        PRINT "Pass"
    Else
        PRINT "Fail"
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input averageMark/]
    B --> C{"averageMark >= 50"}
    C -->|Yes| D[/"Print #quot;Pass#quot;"/]
    C -->|No| E[/"Print #quot;Fail#quot;"/]
    D --> F([End])
    E --> F
```

---

## 9. Calculate Factorial of a Number

Write the algorithm and draw the flowchart that input a number and calculate its **factorial** using a loop. (5! = 5 × 4 × 3 × 2 × 1)

### ✔ Pseudocode

```text
START
    INPUT n
    total = 1
    FOR i = 1 TO n
        total = total * i
    ENDFOR
    PRINT total
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input n/]
    B --> C[total = 1]
    C --> D[i = 1]
    D --> E{"i <= n"}
    E -->|No| F[/Print total/]
    E -->|Yes| G[total = total * i]
    F --> H([End])
    G --> I[i = i + 1]
    I --> E
```

---

## 10. Calculate Discount on Purchase

Write the algorithm and draw the flowchart for a program that inputs the purchase amount and gives a **10% discount** if the amount is **greater than 1000**.

### ✔ Pseudocode

```text
START
    INPUT amount
    IF amount > 1000
        amount = amount * 0.9
        PRINT amount
    Else
        PRINT amount
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input amount/]
    B --> C{"amount > 1000"}
    C -->|No| D[/Print amount/]
    C -->|Yes| E[amount = amount * 0.9]
    D --> F([End])
    E --> D
```

---
