
# Verkefni 5 - 15%
---

<!--
1. [Electronics Class](https://www.instructables.com/Electronics-Class/)
1. [Robot class](https://www.instructables.com/Robots-Class/)
-->

<!--
All you need to control a motor using an Arduino is a 2K resistor, an NPN transistor (TIP120 in this case), and a 1N4001 diode. The 2K resistor works to protect the Arduino pin, the transistor serves as a valve which lets more or less current flow through the motor. This is what turns the motor on and off, and controls its speed.

The diode is used as a buffer. When electricity flows through the motor, the diode does nothing. However, when the motor stops, the reverse current flows across the diode, and back through the motor. This protects the circuit from sudden voltage spikes.
-->

### 5.1 Mótorar og hreyfingar. (1%)
Lestu um algenga mótora og hreyfingar í [Motors and Motion](https://www.instructables.com/Motors-and-Motion/)

1. Hvernig er stýrimótor (e. servo motor) ólíkur hefðbundnum DC mótor?
1. Hvernig er hægt að stjórna í hvora áttina DC mótor snýst án kóða?

<!--
[samanburður á DC,stepper og server](https://www.seeedstudio.com/blog/2019/03/04/driving-a-28byj-48-stepper-motor-with-a-uln2003-driver-board-and-arduino/)
-->
---

### 5.2 Servo Motors 
1. Lestur þig til um [Servo mótors](https://www.instructables.com/Servo-A-Go-Go/)
2. Myndband (1 mín) sem sýnir innviði stýrimótors [inside a servo motor](https://learn.adafruit.com/adafruit-arduino-lesson-14-servo-motors/inside-a-servo)

---

### 5.3 Servo Motors & `Sweep` forritið (3%)
Kynntu þér hvernig Servó mótor virkar og settu upp og keyrðu `sweep` kóðann á brauðbretti [Sweep leiðbeiningar](https://lastminuteengineers.com/servo-motor-arduino-tutorial/#arduino-code-sweep)

_Hvað snýst servo motor margar gráður þegar hár púls (e. pulse) varir í 1.5 millisekúndur?_

---

### 5.4 Rafþéttar (e. capasitors) (1%)
Kynntu þér rafþétta (e. capasitors):
1. [Circuit Playground: C is for Capacitor (myndband, 7 mín.)](https://learn.adafruit.com/circuit-playground-c-is-for-capacitor/video)
2. [Capacitors](https://www.instructables.com/lesson/Capacitors-2/)

_1. Hver er munurinn á rafhlöðu og rafþétti?_<br>
_2. Hver er munurinn á Nonpolarized (NPD) og polarized (PD) þéttum?_
_3. Afhverju er heppilegt að nota rafþéttir með mótor?_

<!--
Sometimes your servo may misbehave if you decide to run it directly from the Arduino. The reason for this is that the servo draws considerable power, especially during start-up, and this can cause the Arduino board to reset.
-->

---

### 5.5 Controlling Servo with a Potentiometer (3%)
Settu upp og keyrðu `Knob` kóðann á brauðbretti, notaðu þéttir, sjá [Knob leiðbeiningar](https://lastminuteengineers.com/servo-motor-arduino-tutorial/#controlling-servo-with-a-potentiometer)

_Hvað gerir `map` fallið? í kóðanum?_

---

### 5.6 Skrefamótorar (e. stepper motors) (1%)
1. [How does a Stepper Motor work? (6 mín myndband)](https://www.youtube.com/watch?v=eyqwLiowZiU)
1. [How to use Stepper motors (7 mín myndband)](https://youtu.be/bkqoKWP4Oy4). 

1. _Hvernig er skrefamótor ólíkur hefðbundnum DC mótor?_
2. _Nefndu dæmi þar sem skrefamótorar nýtast betur en aðrar gerðir mótora._

---

### 5.7 Control 28BYJ-48 Stepper Motor with ULN2003 Driver & Arduino (3%)
1. Lestu og kynntu þér [Control 28BYJ-48 Stepper Motor with ULN2003 Driver & Arduino](https://lastminuteengineers.com/28byj48-stepper-motor-arduino-tutorial/)
2. Settu upp á brauðbretti og keyrðu etirfarandi forrit í Arduino IDE: `File -> Examples -> Stepper -> stepper_oneStepAtATime`

#### Punktar:
- **EKKI** tengja stepper motor við 5V á Arduino. 
- Powering the stepper motor directly from the Arduino can damage it!
- Notaðu 5V DC power supply fyrir skrefamótor.

Wiring diagram:

![Wiring diagram](https://github.com/VESM1VS/V21-1/blob/main/Myndir/28BYJ-48-Stepper-Motor-ULN2003-Driver-Wiring-Diagram-Schematic-Pinout.jpg)

---

### 5.8 Skrefamótor og AccelStepper safnið (3%)
Fylgdu [kóðasýnidæmi með `AccelStepper` safni](https://lastminuteengineers.com/28byj48-stepper-motor-arduino-tutorial/#arduino-code-using-accelstepper-library) og settu upp á Breadboard. 
<br>
- It supports acceleration and deceleration.
- It supports half-step driving.
- It supports multiple simultaneous steppers.

<!--
[Fleiri dæmi](https://www.makerguides.com/28byj-48-stepper-motor-arduino-tutorial/)
when powering the Arduino with USB power only, I would get inconsistent behavior and bad performance of the stepper motor.
-->

---

### 5.9 DC Motors 
[DC Motor, How it works? (5 mín myndband)](https://www.youtube.com/watch?v=LAtPHANEfQo&vl=ko)

---

## Námsmat og skil

Búðu til í **private** Github Repository vefsíðu í wiki eða skrá með markdown sniði (.md) sem inniheldur eftirfarandi:

- Svör við spurningum
- Tengla á myndbönd af verklegum verkefnum. 
  - _Láttu nafnið þitt og dagsetningu koma fram í myndbandinu._
- Tengla á kóðaskrár sem þú notar í verklegum verkefnum (upload kóðaskrár).


<!--

### 5.8 Transistorar 

1. Kynntu þér [Transistora](https://www.instructables.com/lesson/Transistors/).
1. Svaraðu eftirfarandi spurningum:
    1. Hvað gerir transistor?
    1. Hver er munurinn á NPN og PNP transistorum?


#### 5.6 Nánar um ULN2003 & 28BYJ-48 Stepper Motor
5.6 Kynntu þér virkni og möguleika með [ULN2003 & 28BYJ-48 Stepper Motor (myndband)](https://medium.com/jungletronics/uln2003-28byj-48-stepper-motor-f1cc5357eff).

## Control Stepper Motor with L293D Motor Driver IC
- https://lastminuteengineers.com/stepper-motor-l293d-arduino-tutorial/

## DC Motors 
- [DC Motor, How it works? (myndband)](https://www.youtube.com/watch?v=LAtPHANEfQo&vl=ko)

## DC Motors 

1. Fylgdu [Lesson 13. DC Motors](https://learn.adafruit.com/adafruit-arduino-lesson-13-dc-motors) og settu upp á Breadboard:
2. Svaraðu eftirfarandi spurningum:
    1. Afhverju þurfum við að nota PWM pinna til að stýra DC mótor?
    2. Afhverju þurfum við að nota viðnám, transistor og diode með DC mótor?
    3. Hvernig er stýrimótor (e. servo motor) ólíkur hefðbundnum DC mótor?


## H-Bridge 
To make a motor spin backwards, you will need an H-bridge.

1. Lestu þér til um [L293D H-Bridge](https://maker.pro/custom/projects/all-you-need-to-know-about-l293d).
1. Svaraðu eftirfarandi spurningum:
    1. Hvað er hægt að gera með L293D?
    1. Hver er munurinn á L293 or L293D?


## DC motor reversing 

1. Fylgdu [Lesson 15. DC Motor Reversing](https://learn.adafruit.com/adafruit-arduino-lesson-15-dc-motor-reversing) og settu upp á Breadboard.

1. Svaraðu eftirfarandi spurningum:
    1. Útskýrðu virkni eftirfarandi falls:

        ```cpp
        void setMotor(int speed, boolean reverse) {
            analogWrite(enablePin, speed);
            digitalWrite(in1Pin, !reverse);
            digitalWrite(in2Pin, reverse);
        }
        ```
    1. L293D er með tvo +V pinna (8 and 16), útskýrðu þá.

Ítarefni: [Tveir DC mótorar: speed and spinning direction of a DC motor](https://lastminuteengineers.com/l293d-dc-motor-arduino-tutorial/)

-->

