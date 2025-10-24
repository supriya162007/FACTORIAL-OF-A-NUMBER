# FACTORIAL-OF-A-NUMBER-USING-8051-KEIL

**AIM:**

To write and execute Assembly language Program to perform factorial of a number using 8051 keil.
APPARATUS REQUIRED: Personal computer with Keil software

**ALGORITHM:**

• Start  

• Input: Read the number n.  

• Initialize:  

•Set factorial to 1.  

•Set i to 1.  

• Loop: While i is less than or equal to n:  

•Multiply factorial by i.  

•Increment i by 1.  

• Output: Store or print the value of factorial.  

• End

**FLOW CHART:**
<img width="261" height="308" alt="image" src="https://github.com/user-attachments/assets/bffe89f6-3ba9-4294-b817-8b545f680e66" />

**Program:**

ORG 0000H   

MOV A,#04H  

MOV R0,A  

ACALL FACTORIAL  

MOV 40H,A  

SJMP THIN  

FACTORIAL:DEC R0  

CJNE R0,#01H,PRODUCT  

SJMP THICK   

PRODUCT:MOV B,R0  

MUL AB  

ACALL FACTORIAL  

THICK: RET  

THIN:  

END

**Output:**  
<img width="1919" height="1134" alt="Screenshot 2025-10-22 182938" src="https://github.com/user-attachments/assets/be6276cb-ff45-4dfe-80f2-bd461a874feb" />



**Manual Calculations:**  

![WhatsApp Image 2025-10-24 at 08 56 00_0570e774](https://github.com/user-attachments/assets/fcf8faa2-725b-465b-b312-08f2acf16cf7)






**Result:**

Thus the factorial of a number using 8051 keil was calculated and shown the output.
