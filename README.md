# H5-palvelinten-hallinta

## Hello Windows -salt

Ensiksi tein hakemiston \tmp\srv\salt, sinne hakemiston hello johon tein init.sls tiedoston
```
C:\Users\ttrbe>mkdir c:\Users\ttrbe\tmp\srv\salt   
c:\Users\ttrbe\tmp\srv\salt>mkdir hello
c:\Users\ttrbe\tmp\srv\salt>type NUL > init.sls

```
Tarkastin, että kaikki tuli tehtyä oikein.
```
c:\Users\ttrbe\tmp\srv\salt>dir

01.12.2022  07.05    <DIR>          .
01.12.2022  06.52    <DIR>          ..
01.12.2022  07.02    <DIR>          hello
01.12.2022  07.05                 0 init.sls
               1 File(s)              0 bytes
               3 Dir(s)  230 033 870 848 bytes free
```
Kyllä, kaikki ok. Seuraavaksi init.sls sisältö
```
c:\Users\ttrbe\tmp\srv\salt>notepad init.sls
c:\Users\ttrbe\tmp\srv\salt>type init.sls

C:\Users\ttrbe\tmp\srv\salt\hello\suolaikkuna.txt:
  file.managed:
```
***en saanut salttia asennettua -> opettelen myöhemmin***

## B - Tekniset tiedot tekstitiedostoon

Ensiksi tein juureen temppi-hakemiston, menin hakemistoon ja otin listauksen
```
c:\>mkdir temppi

c:\>cd temppi

c:\temppi>dir
 Volume in drive C has no label.
 Volume Serial Number is FE35-AB7E

 Directory of c:\temppi

01.12.2022  07.31    <DIR>          .
               0 File(s)              0 bytes
               1 Dir(s)  230 012 628 992 bytes free
```
Koneen tiedot sain systeminfo-komennolla '>' ohjaa tulosteen tiedostoon
```
c:\temppi>systeminfo > systeemi.txt

c:\temppi>dir
 Volume in drive C has no label.
 Volume Serial Number is FE35-AB7E

 Directory of c:\temppi

01.12.2022  07.32    <DIR>          .
01.12.2022  07.32             3 178 systeemi.txt
               1 File(s)          3 178 bytes
               1 Dir(s)  230 011 510 784 bytes free

```
