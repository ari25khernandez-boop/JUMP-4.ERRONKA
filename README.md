# JUMP-4.ERRONKA
     
## AUTOMATA PROGRAMAGARRIAK

<img width="717" height="912" alt="0" src="https://github.com/user-attachments/assets/b75caa8b-b0c2-4f37-a7f0-c7c9da629a3a" />

  Taldearen Izena: JUMK S.L
  
Taldekideak: Karen H, Jon O, Unax A eta Maddi U.

AURKIBIDEA:
<ul>
    
1 SARRERA	

2 PROIEKTUAREN JATORRIA ETA TESTUINGURUA	

3 HELBURUAK

4 AUTOMATISMOA	
 - CADE-SIMU	
 - FUNTZIONAMENDUA	
      
5 ABIARAZLE PROGRESIBOA	
 - ABIARAZLE  ZUZENA:
 - IZAR-TRIANGELU ABIARAZTEA(∆/ㄚ):
 - ABIARAZLE  PROGRESIBOA:	
 
6  ARDUINO	
<p>
7 DIGITALIZAZIOA
 - EXCEL
 - K3GN PANTAILAREN KONFIGURAZIOA
 - DATASHEET	
</p>
8  IRAUNKORTASUNA	

9  OSAGAIAK
 - ULTRASOINUA
 - DIFERENTZIALA
 - SEGURTASUN-MODULUAK
 - ERRELE LAGUNTZAILEA
 - MAGNETOTERMIKOA
 - POTENTZIA-KONTAKTOREA
 - DISYUNTOREA
 - ABIARAZLE PROGRESIBOA  

10  AURREKONTUA	

11  BIBLIOGRAFIA	

12  BIDEOA	

13  ANEXOAK
 - AUTOMATISMOAREN ESKEMA	


## **SARRERA**
<br>


#### **HELBURUAK**
Proiektu honen helburua Cade-Simuko eskema elektriko bat egitea da , hau da, eskemak egiten dakigula erakustea eta guk behar ditugun elementuak egotea eta beraien arteko kableatua egokia izatea. Cadesimuko eskema ikusita gai izan behar gara automatismoaren muntaia egiteko eta mantenimentua egokia emateko. Programazioaren eskuliburua ikusita maiztasun bihurgailuaren parametroak sartzen ikasi dugu eta PLC arekin komunikatzen. Horrezgain, arduinoren bitartez motorraren temperatura kontrolatu ahal dugu bertan DHT11-ren laguntzarekin kontrolatzen baina leh duguenago, nola erabiltzen den eta nola programatu behar den ikasi genuen. Arduinorekin batera PLC-aren zekuentzia programasioan gehiago ikasi dugu eta zirkuituan pasatzen dena HMI pantallan adieraztea eta bere programazioa.


#### **AUTOMATISMOA**
<ul>
      FUNTZIONAMENDUA:
      
Gure zirkuitu asteko lehenik eta behin entxufea konektatua egin behar da, bere diferentziala eta magneto-termikoa elektrizitatea pasatzen itxi behar du. Emerentziako zeta eta segurtasuneko ibiltarte amaiera On egoeran badaude Segurtasun Errelea aktibatu egingo da eta PLC-ko Sarrera eta Irteeretara  elektrizitatea heltzeko Aukera histen du. Botoi berdea sakatzen dugun bitartean I.0.1 bariablea piztu egiten da eta PLC barruan programaren barruan señale hori memoria barruan gelditzen da. Martxa Bariablea, A0 Detektorea, B0 Detektorea, Induktibo 1 elementual Sarreretako Bariableak badaude B zilindroak kanpora egingo du Y1 solenoidearekin, B1 Detektorea seinalea ematen duenean eta Sentsore Foto-elektrikoa detektatzen badu denbora bat pasatzerakoan Y1 solenoideak elektrizitatea kentzen da eta B zilindroa barrura itzuliko da B0 berriro here detektatzerakoan platikozko pieza baldin bada ezkerrera mugitzen hasiko da pieza motor baten laguntzarekin FC1 ibiltate amaiera ikutzerakoan motorra gelditu egiten da, zagoen pieza kentzen dugunean denbora bat pasatu ostean motorra eskumatara biratzen hasiko da Induktibo 1 detektatu arte hor gelditu egiten da. Hasierako egoera berriro here betetzen direnean zekuentzia berriro here hasi egingo da B zilindroa kanpora ateratzen, B1 detektatzerakoan eta Sensore Foto-Elektrikoa detektatzen du baina oraingoan Induktibo 2 ere detektatzen du burdinezko pieza bat detektatzen duelako. B zilindroa atzera itzultzerakoan B0 detektagailuak seinalea ematen du eta pieza eskumatara mugituko da motorraren laguntzarekin FC2 ibiltarte amaierara heltzerakoan motorra gelditu egiten da. Denbora bat pasatu ostean eta burdinezko pieza kentzen denean motorra ezkerrera bidali dugu. Lehenengo zutabetik 4 piezak ateratzen direnean A zilindroak A+ pozisiora joango da Y3 solenoidearen laguntzarekin. 4 aldiz berriro ere egiten denean A zilindroa A- pozisioara joango da Y4 solenoidearekin.
      
</ul>

