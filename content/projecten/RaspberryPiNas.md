---
title: Raspberry Pi Nas
type: projecten
date: 2021-09-06
tags: 
    - Eigen
---

In het eerste jaar van mijn bachelors opleiding kregen we het vak IoT Essentials. Bij dit vak werden we verplicht om een Raspberry Pi aan te schaffen.
Na het slagen van dit vak vond ik het zonde om hier dan niets meer mee te doen aangezien het toch een nuttig stukje hardware kan zijn.

Daardoor ben ik op zoek gegaan naar verschillende projecten die ik er mee zou kunnen realiseren.

Toen stoote ik op een video van NetworkChuck op Youtube. Hierin maakte hij van zijn Raspberry Pi een Nas waarmee je niet alleen lokaal maar ook remote mee kon verbinden.

Aangezien ik de Pi toch niet gebruikte en ik nog een externe HDD had liggen van 4Tb die niet gebruikt werd. Dacht ik dat dit het ideale project was.


In dit project leer je hoe je een Pi klaarmaakt voor gebruik door er een OS op te zetten. Ik had gekozen voor de Raspberry Pi OS Lite image.
Met het gebruik van de Raspberry Pi Imager was dit process heel makkelijk en daardoor kon ik ookal op voorhand SSH en andere instellingen configureren.

Natuurlijk is de basis kennis van linux nodig, deze had ik gelukkig al door zowel het vak Linux Essentials als IoT Essentials.

Na het voorbereiden van de Pi, installeerde ik OpenMediaVault.
Vanaf dat OMV geïnstalleerd staat kan je via je browser connecteren met je PI met het IP adres.
Nu dat OMV op je Pi staat begin je met de configuratie.

In de configuratie mount je, je HDD, maak je een shared folder, dit is uiteindelijk de folder waar je toegang tot krijgt in je NAS. 

Als dit gedaan is moet je, je service kiezen. Ik koos hierbij voor SMB aangezien ik windows gebruik.
Om dit aan te zetten is het met OMV heel simpel te doen door gewoon de enable slider aan te zetten en dan je shared folder te kiezen.

Vanaf dit moment is het gewoon een netwerk locatie toevoegen met het IP adres van je PI met dan de naam van je shared folder.
Aan de hand van welke users je geconfigureerd hebt moet je een username en wachtwoord ingeven, en dan kan je aan je files.

Natuurlijk is het leuk om lokaal aan mijn files te kunnen maar dan kan ik even goed de HDD rechtstreeks connecteren aan mijn pc.
Dus ging ik een stapje verder, ik maakte het ook mogelijk om remote aan mijn bestanden te kunnen met de FTP server.

Uiteindelijk had ik voor elk gezinslid een shared folder gemaakt en hadden we een basic private cloud.

Door dit project heb ik wat meer kennis gekregen over de basisprincipes van netwerken zoals port forwarding en netwerkconfiguratie.
Daarnaast wat meer kennis over opslagbeheer en de verschillende bestandssystemen zoals ext4 en NTFS.

![Alt text](/images/raspberry-pi-nas-1.png)
![Alt text](/images/raspberry-pi-nas-2.png)
