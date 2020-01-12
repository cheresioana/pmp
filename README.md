# pmp
Proiectare cu microprocesoare
##Robot care ocoleste obstacole

1. Schema
   ![](images/robot.jpg)
2. Utilizare
   - Se ruleaza codul in Arduino si se urca pe placuta. Mai departe robotul ruleaza independent.
3. Componente
   - Placa Arduino uno
   - Senzor ultrasonic
   - Servo
   - Doua motoare
   - H-bridge
4. Explicatii

   - Senzorul ultrasonic trimite un semnal, care este controlat de trigPin. Acesta asteapta pana cand unda se intoarce, iar senzorul returneaza timpul intre momentul in care s-a trimis semnalul si momentul in care a receptionat intoarcerea semnalului. Stiind viteza cu care este propagata unda (viteza sunetului) si timpul, se poate calcula distanta parcursa.
   - distanta = viteza * timp
	- In functie de distanta la care se afla obiectul in fata robotului acesta poate sa: mearga in fata, vireze la dreapta, vireze la stanga.
