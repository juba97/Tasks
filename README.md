> **C# includes some predefined value types and reference types. The following table lists predefined data types:**  
                                                                                     
![](https://www.theengineeringprojects.com/wp-content/uploads/2018/02/introduction-to-data-types-in-C-1.png)

 ```C#
        int i;
        i = 0;

        bool someCondition = false;
        
        // Here, i is still incremented even though the if statement fails.
        if (someCondition & (i++ < 100))
        {
            Console.WriteLine("this won't be displayed");
        }
        else
        {
            Console.WriteLine("if statement executed: " + i); // displays 1
        }
          // In this case, i is not incremented because the short-circuit
         // operator skips the increment.
        if (someCondition && (i++ < 100))
        {
            Console.WriteLine("this won't be displayed");
        }
        else
        {
            Console.WriteLine("if statement executed: " + i);  // still 1 !!
        }
```

|    P   |    Q   | P implies Q |                    
|--------|--------|-------------|
| True   | True   | True          
| True   | False  | False         
| False  | False  | True  
| False  | True   | True  
