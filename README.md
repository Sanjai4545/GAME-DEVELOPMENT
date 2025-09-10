## EX 1: DDA ALGORITHM 

**Aim :**

To  implement the DDA algorithm to draw a line using a c coding

**Algorithms :**

Step 1 − Get the input of two end points (X0,Y0) and (X1,Y1)

Step 2 − Calculate the difference between two end points dx and  dy 

Step 3 − If dx > dy, then you need more steps in x coordinate; otherwise in y coordinate.

Step 4 − Calculate the increment in x coordinate and y coordinate

Step 5 − Plot the pixel by successfully incrementing x and y coordinates accordingly and complete the drawing of the line

**Program :**

```
initgraph(&gd,&gm,"c:\turboc3\bgi");
 printf("Enter the value of x1 and y1 : ");
 scanf("%f%f",&x1,&y1);
 printf("Enter the value of x2 and y2: ");
 scanf("%f%f",&x2,&y2);
 dx=abs(x2-x1);
 dy=abs(y2-y1);
 if(dx>=dy) step=dx; else step=dy;
 dx=dx/step; dy=dy/step;
 x=x1; y=y1;
 i=1;
 while(i<=step)
 { putpixel(x,y,5);
 x=x+dx;
 y=y+dy;
 i=i+1;
 delay(100);
 }
```

**Output :**
<img width="794" height="623" alt="image" src="https://github.com/user-attachments/assets/8657b0dd-5dff-40df-b289-470e9b434b61" />

**Result :**

 Thus the DDA algorithm to draw a line using a c coding is implemented successfully.
