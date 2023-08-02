---
layout: single
title: "Demonstrator värmekamera"
---

MLX90640 är en värmekamera som utvecklats av Melexis, ett mikroelektronikföretag baserat i Belgien. Den är designad för att detektera långvågig infraröd strålning som föremål naturligt avger och omvandla det till en visuell representation av temperaturen.

MLX90640 har en matris med 32x24 pixlar, vilket innebär att den kan detektera 768 olika temperaturavläsningar samtidigt. Den har ett synfält på antingen 55° eller 110° och kan detektera temperaturer från -40°C till 300°C. Noggrannhet i temperatur är typiskt 1°. 

Sensorn används vanligtvis i olika tillämpningar såsom byggnadsautomatisering, processkontroll, medicintekniska enheter och fordonsapplikationer. Den är också populär bland hobbyister och makers för dess användarvänlighet och prisvärdhet jämfört med andra värmekameror.


![MLX90640](https://media.melexis.com/-/media/images/product-media/mlx90621/mlx90621-far-infrared-array-melexis.jpg)
*Figur 1 - Melexis MLX90640 värmekamera litet format med 32x24 pixlar.*

![[mlx90640-pen-crop.jpg]]
*Figur 2 - MLX90640 monterad på ett kretskort.*

I vår demonstrator styrs kameran av en mikrokontroller (RP2040) som sedan skickar datan vidare över WiFi så att man kan ta emot och visualisera den på en dator. Programmet på mikrokontrollern är skrivet i C++ och programmet på PC eller Mac för visualisering är skrivet i Python.

För att visualisera information från en värmekamera brukar man använda *falsk färg*, vilket betyder att man använder en färgskala eller en gråskala där olika nyanser får representatera olika temperaturer. På detta sätt kan man göra det enkelt att se variationer i temperatur och framhäva föremål som är varmare eller kallare än de borde vara.

![[thermal-image-hand.jpg]]
*Figur 3 - En hand fotograferad av värmekameran och visualiserad med falsk färg.*

[Termografi](https://en.wikipedia.org/wiki/Thermography) är en teknik som används för att mäta och visualisera temperaturförändringar på ytor med hjälp av värmekameror eller termiska avbildningssystem. Genom att mäta och analysera infraröd strålning som utstrålas från olika föremål eller ytor kan termografi användas för att upptäcka avvikelser från normala temperaturmönster. Termografi kan användas inom många områden som byggnads- och fastighetsunderhåll, inspektion av elektriska anläggningar, medicin, tillverkningsprocesser och mycket mer. Genom att upptäcka temperaturavvikelser i realtid kan termografi hjälpa till att identifiera potentiella problem eller fel innan de leder till mer allvarliga skador eller kostsamma reparationer.

Läs mer på [Melexis MLX90640 produktsida](https://www.melexis.com/en/product/MLX90640/Far-Infrared-Thermal-Sensor-Array).
