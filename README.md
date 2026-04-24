# JUMP-4.ERRONKA
     
## AUTOMATA PROGRAMAGARRIAK

<img width="717" height="912" alt="0" src="https://github.com/user-attachments/assets/b75caa8b-b0c2-4f37-a7f0-c7c9da629a3a" />

  Taldearen Izena: JUMK S.L
  
Taldekideak: Karen H, Jon O, Unax A eta Maddi U.
<ul>
   AURKIBIDEA:

   - SARRERA:
        - ESKEMA
             - CAD-e SIMUS
             - TIA PORTAL

   - PROGRAMA (arduino)

   - ATV320

   - IRUZKINAK
     
     
</ul>


## **SARRERA**

Gure enpresa JUMK S.L.  zinta banatzaile maketen instalazio elektroneumatikoetan zentratzen da. Bertan elementu metaliko eta ez diren banaketa egokia egiten du. Horretrako PLC1200, ATV230 eta arduino mikropogramatzailea erabiltzen dira.

Maketan funtzio nagusia honakoa da. HMI pantailan guk nahi ditugun pieza kopurua erabakiko degu eta horren arabera piezak klasifikatzen joango da zinta bitartez eskubiruntz edo ezkerreruntz. 


## **OSAGAIAK**

Maketa hau egiteko alde batetik elemtu fisikoak (hadware) eta ez fisikoak (software) erabili dira.

* SOFTWARE:
  - TIA PORTAL
  - CADe_SIMUS
  - PC_SIMUS
  - FLUID-SIM
  - ARDUINO IDE
  - LUCIDCHART
  - CISCO PACKET TRACE 
  
* HADWARE:
   - PLC 1200
   - ARDUINO
   - ATV320
   - MOTORRA


## ESKEMA

Alde bateik ikus daiteke maketan funtzionamendu nagusirako grafcet bat daukagula. Bertan ziklo hau betetzen da. 

Hasteko nahi den pieza kopurua erabakiko da zenbat metaliko edo ez metaliko HMI pantaila bitartez. Orduan martxan jarrita maketa zilindro batek pieza aterako du zintara eta bertan daude sentsoreek detektatzean PLC-ak informazio hori prozesatu eta eskubi (ez metalikoa) edo ezkerrera (metalikoa) bideratuko du pieza. 

Horrezgain…(grafcetari almazena beteta falta zaio)

Bestalde emergentzirako grafcet-a irudikatzen da non seta, paro edo motorran tapan egoera aldatzen bada, zikloa guztiz gelditzeko. 


<img width="1039" height="511" alt="Captura" src="https://github.com/user-attachments/assets/634bbcf5-6145-4f21-a6b8-0faf1bfcc1d9" />



Motorra martxan jartzeko temperatura-muga bat ezarri zaio zenbakizko teklatu baten bitartez. Gero ere LCD pantaila baten bidez motorran tenperatura erreala bistaratuko da eta ezarri den tenperatura muga gainditzen bada bertan mezu bat agertuko da «Temperatura muga gainditua». Muga hau gaindituz seinale bat bidaliko du PLC-ra.


<img width="1875" height="2344" alt="4  ERRONKA  - Page 1_page-0001 (1)" src="https://github.com/user-attachments/assets/a2a08a26-f76c-4b0a-97c1-516b3baf8c7c" />


## **PROGRAMAK**

* GRAFCET
  
     Alde bateik ikus daiteke maketan funtzionamendu nagusirako grafcet bat daukagula. Bertan ziklo hau betetzen da. 

     Hasteko nahi den pieza kopurua erabakiko da zenbat metaliko edo ez metaliko HMI pantaila bitartez. Orduan martxan jarrita maketa zilindro batek pieza aterako      du zintara eta bertan daude sentsoreek detektatzean PLC-ak informazio hori prozesatu eta eskubi (ez metalikoa) edo ezkerrera (metalikoa) bideratuko du pieza. 

     Horrezgain…(grafcetari almazena beteta falta zaio)

     Bestalde emergentzirako grafcet-a irudikatzen da non seta, paro edo motorran tapan egoera aldatzen bada, zikloa guztiz gelditzeko.
       <foto de grafcet>


## **ATV320**

Motorran abiadurak eraldatzeko bariadore hau erabilida. Horretarako bere manualeko parametroak gure maketera egokitzen diren datuetara egokitu dira. 

Parametros de fabrica


|  DRI->  |  CONF->    | FCS-> |    |
| ------------ | ------------ | ------------ | ------------ |
|   |   | FRY->  |   |
|   |   |   | >ALL"  |
|   |   | GFS ->   |  YES(2s) |


Velocidad preseleccionada

| DRI-> | CONF->   | FCS->  | FULL>  |FUN|   |
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ |
|   |   |   |   | PSS> |   |
|   |   |   |   | >PS2  |  LI3 |
|   |   |   |   |> PS4 |  LI4 |
|   |   |   |   | >SP2  |  15Hz |
|   |   |   |   |  >SP3 | 20,5Hz  |
|   |   |   |   | >SP4  |  30Hz |


parametros del motor

|  DRI-> |  CONF-> | FCS->  |  SIM> |   |
| ------------ | ------------ | ------------ | ------------ | ------------ |
|   |   |   |   >tCC  |  2hilos (2s) |
|   |   |   |  >CFG  | Sts |
|   |   |   |   >bFr  | 50Hz   |
|   |   |   |   >nPr  |  0,18Kw |
|   |   |   |  >unS  | 230v  |
|   |   |   |   >nCr  | 0,96A  |
|   |   |   |   >frs |  50Hz  |
|   |   |   |   >nSP | 1310  |


lac

ABIADURA MAX. ETA MIN.

| DRI->  | CONF->  | FULL>  | SIM >|   |
| ------------ | ------------ | ------------ | ------------ | ------------ |
|   |   |   | HSP>  | 0.0  |
|   |   |   | LSP>  | 41  |


2 hilos

|  DRI-> | CONF->  |  FULL> |   |   |
| ------------ | ------------ | ------------ | ------------ | ------------ |
|   |   |  I_O >|   |   |
|   |   |   | L1>  |   |
|   |   |   | LIA> | FRD  |
|   |   |   |  L2 >| LIx |

## **BIDEOA**

<LINK/URL>












