# Logical Operation

## AIM:

To Perform logical operation using Arduino UNO Controller.

## Software required:

Arduino IDE </br>
Proteous 

## PROCEDURE:
### Arduino IDE
Step1:Open the Arduino IDE </br>
Step2: Go to file and select new file option</br>
Step3:Type the program</br>
Step4:Go to file and select save option to save the program</br>
Step5:Go to sketch and select verify or compile options</br>
Step6:If no error Hex file will be generated in the temporary folder</br>
### Proteus 
Step7:Open the Proteus software</br>
Step8:Go to file select new design and click ok button</br>
Step9:Select component mode and click pick devices from the library</br>
Step10:Type the component name in the keyword to select the components and click ok button</br>
Step11:Design the circuit as per the diagram</br>
Step12:Double click the Arduino controller and upload the hex file generated by Arduino IDE</br>
Step13:Click start button and check the output</br>
## THEORY:
Logic gates are the basic building blocks of any digital system. It is an electronic circuit having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as AND gate, OR gate, NOT gate etc.

![image](https://user-images.githubusercontent.com/71547910/235332137-a4a37a0e-ddfb-4ca2-82e5-b1565d969413.png)

![image](https://user-images.githubusercontent.com/71547910/235332175-5d9df189-c964-45d1-ad24-e0afe6ff7eea.png)

![image](https://user-images.githubusercontent.com/71547910/235332188-bff0b03e-1b6a-4de6-993b-20497c247f17.png)

![image](https://user-images.githubusercontent.com/71547910/235332203-6bc16144-762e-40e8-ad6d-f76833a7fca4.png)

![image](https://user-images.githubusercontent.com/71547910/235332217-f598b1fb-78b6-497e-9e0e-ee2bb4dbeb71.png)

![image](https://user-images.githubusercontent.com/71547910/235332241-dd9ce66a-0e77-44d9-a699-09bfbd1968ea.png)

![image](https://user-images.githubusercontent.com/71547910/235332254-db13d222-1246-4b57-bbb2-3ab2287ccaa8.png)

## PROGRAM:
```
int bs0 = 0;         // variable for reading the pushbutton status
int bs1 = 0;
int bs2 = 0;         // variable for reading the pushbutton status
int bs3 = 0;
int bs4 = 0;         // variable for reading the pushbutton status
int bs5 = 0;
void setup() {
  pinMode(13, OUTPUT);
  pinMode(0, INPUT);
  pinMode(1, INPUT);
  pinMode(2, INPUT);
  pinMode(3, INPUT);
  pinMode(4, INPUT);
  pinMode(5, INPUT);
}
void loop() {

  bs0 = digitalRead(0);
  bs1 = digitalRead(1);
  bs2 = digitalRead(2);
  bs3 = digitalRead(3);
  bs4 = digitalRead(4);
  bs5 = digitalRead(5);

  if (bs4 == 0 && bs5 == 0) 
  {
      digitalWrite(13, bs0);
  } 
  else if (bs4 == 0 && bs5 == 1) 
  {
    
    digitalWrite(13, bs1);
  }
   else if (bs4 == 1 && bs5 == 0) 
  {
    
    digitalWrite(13, bs2);
  }
   else   if (bs4 == 1 && bs5 == 1) 
  {
      digitalWrite(13, bs3);
  } 
}
```

## CIRCUIT DIAGRAM:

![image](https://github.com/MIRUDHULA-DHANARAJ/Logical-operation/assets/94828147/4851bc5b-bf92-42d7-92c0-a10e53b108c8)

## OUTPUT:

![image](https://github.com/MIRUDHULA-DHANARAJ/Logical-operation/assets/94828147/8aa5488c-0e95-4e6e-925f-93ac4c7613b8)

## RESULT:

Thus the logical operation was performed by Arduino UNO controller
