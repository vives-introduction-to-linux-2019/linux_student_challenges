# Chapter 10 - RPi Operating System

Download `Raspbian Buster with desktop` en kopieer de image naar de SD kaart.

Boot de Raspberry Pi met toetsenbord, muis en scherm.

Configureer het systeem tot het operationeel is.

Controleer of de gegevens in de cursus van CPU overeenkomen met de gegevens aangegeven in `/proc/cpuinfo`.

Hoeveel RAM heeft de RPi, hoe kan je dit controleren?

Start `raspi-config` als root en configuur de time-zone, wifi en hostname. Enable ook SSH. Plaats screenshots van je resultaat in dit verslag.

Pas het wachtwoord van de user Pi aan. Test dit uit door aan te loggen.

Met welk commando kan je de temperatuur van de CPU opvragen?

Met welk commando vraag je het IP adres op van de RPi? Noteer alvast jouw MAC adres hier.

Gebruik Putty om via SSH te connecteren naar de Pi.

Maak een nieuwe gebruiker aan op je Pi voor jezelf. Zorg dat je kan aanloggen via SSH zonder dat je jouw wachtwoord moet ingeven.

Maak een SAMBA share op de Pi. Doe dit voor je eigen account en share een directory `projects` onder je eigen home. Zorg dat je deze kan bereiken vanop Windows.