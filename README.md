LOC za sve fajlove - 214
Ciklomatska slozenost metoda evaluateExpression je 12 a Calculate takodjer 12.
Kognitivna slozenost metoda evaluateExpression i Calculate:
•	Kognitivna slozenost metode evaluateExpression je relativno visoka. Metoda obavlja vise koraka kako bi izracunala rezultat. Metoda mora obrađivati različite aritmeticke operacije u unesenom izrazu tako da je slozenost jos veca.
•	Kognitivna slozenost metode Calculate je visoka. Metoda obradjuje matematicke operacije sabiranje, oduzimanje, mnozenje, dijeljenje i obradjuje liste numbers i operations kako bi izracunala konacan rezultat. Metoda sadrzi dosta if else blokova koji povecavaju kongitivnu kompleksnost metode.

Pregled
- Program je napisan Java programskim jezikom
- Program se sastoji iz dva fajla: Start.java i Calculator.java 
- Program prima unose i ispisuje rezultat putem Start.java klase koja sadrzi glavnu metodu main
- Klasa Calculator.java sadrzi logiku za izvrsavanje matematičkih operacija
- Program je besplatan za koristenje jer ima MIT licencu

Staticka analiza
Calculator.java - line 18 - metodu ‘ToString’ treba preimenovati kako bi se izbjegla zamjena sa metodom ‘toString’ iz super klase "java.lang.Object“
Calculator.java - line 24 - treba preimenovati metodu ‘Run’ da odgovara regularnom izrazu
Calculator.java - line 53 - petlja ‘for’ se moze zamijeniti for-each petljom
Calculator.java - line 70 - promjenjiva ‘textResult’ je suvisna jer nije potrebna za dalju upotrebu u kodu
Calculator.java - line 74 - treba preimenovati metodu ‘Calculate’ da odgovara regularnom izrazu
Calculator.java - line 87 - iz if bloka se moze izdvojiti Calculate(numbers, operations); return; jer ne utice na izvrsavanje uslova
Calculator.java - line 138 - iz if bloka se moze izdvojiti Calculate(numbers, operations); return; jer ne utice na izvrsavanje uslova
Calculator.java - line 183 – return se treba izbaciti
Start.java - line 6 - treba preimenovati promjenjljivu ‘Expression’ da odgovara regularnom izrazu
Start.java - line 8 i 19 - treba zamijeniti upotrebu System.out ili System.err objekata u ovom kodu sa ‘logger’
