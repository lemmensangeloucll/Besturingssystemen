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
 - Rechter muisknop op de 
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTgwNTAzNjY2NywxNDUyOTk4NDg4LC0yMD
k3NDY1NDIsOTk2MTg2NDM1XX0=
-->