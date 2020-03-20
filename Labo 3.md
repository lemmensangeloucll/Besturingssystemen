# Besturingssystemen 1 (MBI10a) - Labo 3

Dit kan worden gebruikt voor Labo 3 van besturingssystemen.
> Belangrijk! Labo 1 en 2 moeten volledig afgerond zijn om aan dit labo te kunnen beginnen.

## README
Deze documentatie is gebaseerd op het labo dat je [hier](https://github.com/swenr/operating-systems/tree/master/Storage%2C%20Shares%20en%20rechten) kan terugvinden.
Sommige teksten zijn gekopieerd.
Er kunnen geen rechten worden ontleend of aansprakelijkheid worden aanvaard.

# Voorbereiding
Voeg aan je Windows Server een extra schijf toe. Dit doe je via VMWare, onder instellingen van de VM.
> Om de schijf te kunnen toevoegen moet je VM wel uit staan!

Als je de schijf hebt toegevoegd, start je de Windows Server weer op.
Je gaat naar Computer Management -> Disk Management.
Je zou dan onderstaan beeld moeten zien.
> Screenshot toevoegen

Er staat nu dat disk 1 offline is, maar we willen hem natuurlijk activeren en kunnen gebruiken.
- Je klikt met je **rechter** muisknop op de disk en klikt op **Online**, zodat deze geactiveerd wordt.

> Screenshot toevoegen

Daarna moeten we nog een volume toevoegen aan de schijf zodat deze bruikbaar is.
- Klik in de **Unallocated** space met je **rechter** muisknop en klik op **New Simple Volume...**.
> Screenshot toevoegen
- Je laat alle standaard waarden staan maar past wel het volgende toe:
   - Drive-letter: M
   - Filesystem: NTFS
   - Label: ShareDisk

# Sharing
 Nu moet de disk gedeeld worden met andere gebruikers op de computer.
 - Open Verkenner
 - Rechter muisknop op de ShareDisk
 - Open het tab Sharing
 - Ga naar Advanced Sharing
 - Vink Share This Folder aan
 - Geef het de naam NetShare
 - Sluit het venster
 - Maak nu een txt bestandje in de schijf om te testen.

Ga naar je Windows client en zoek de share in verkenner en bekijk het bestand.
Kan je het bestand bekijken, bewerken, verwijderen?
> Dit kan je niet, de client heeft enkel lees rechten.

De lector raad aan om volgende [filmpje](https://www.youtube.com/watch?v=GfmkD12ywfw) te bekijken en [deze blog post](https://blog.netwrix.com/2018/05/03/differences-between-share-and-ntfs-permissions/) te lezen en zelf ook dingen ervan uit te voeren.
Zelf raad ik aan [dit filmpje](https://www.youtube.com/watch?v=fJHFmt6F0Rc&list=PLJcaPjxegjBVnEN8c6O8w1mNit4WGeAWN&index=14&t=0s) te bekijken, hierin wordt alles heel duidelijk uitgelegd en met een exacte demo.

## In de praktijk
Om verder te kunnen gaan met het labo moeten we sharing opnieuw uitschakelen op de omgekeerde manier als we het hebben ingeschakeld.

- Ga je naar Server Manager en 
- Ga naar File and Storage Server
- Selecteer Shares
- Je zou dan volgende scherm moeten zien
> Screenshot toevoegen

- Verwijder het tekstbestand uit de share via verkenner
- maak volgende makken aan
  - SalesShare
  - HRShare
  - EngeneeringShare
- Ga terug naar Server Manager ( het scherm in de bovenstaande screenshot)
- Onder Tasks kiezen we voor nieuwe Share 
<!--stackedit_data:
eyJoaXN0b3J5IjpbODU2NzkxODI2LDE0NTI5OTg0ODgsLTIwOT
c0NjU0Miw5OTYxODY0MzVdfQ==
-->