### Vad ska jag göra och hur ser spelet ut? ###
*1* Jag ska göra en hängagubbe spel som använder 75st random ord. 25 enkla, 25 medium svårighet och 25 svåra. 
*2* Spelet ska välja en av 3 svårigheter, "easy", "noraml" eller "hard". Easy ord är korta och enkla medans Hard ord är långa och svåra, normal är i mitten av de 2.
*3* Spelet funkar precis som ett vanligt hängagubbe spel, dvs "bygga" klart gubben för att hänga gubben. Användaren har 6 försök på sig för att gissa ordet spelet har valt.
*4* Om användaren har förlorat så måste hen börja om, om användaren har vunnit så får hen en belöning. Belöningen är att gubben är fri och redo för en till försök.

--=-|-------------------------------------------------------------------------------------------------------------|=--
### Tydligare beskrivning och svar om frågorna koden ###
*1; Vilken extra funktionalitet har du tänkt implementera?*
-  en "difficulty" funktion som bestämmer hur svåra orden ska vara, när spelet börjar så väljer den mellan 3 random svårighetsgrader.

- en "wordCheck" funktion som väljer vilket ord som ska användas ifrån de 75 orden som finns. Den mäter hur lång ordet är som den har valt och lägger "_" så att man vet hur lång ordet är.

- har mindre små funktioner.

*2; Vilka variabler behöver du och till vilket syfte? Här vill jag ha med variabelnamn, datatyp och en förklaring på vad variabeln är till för - på varje variabel.*
-Jag behöver en variabel för ord som senare med funktioner visar hur lång ordet är som man ska gissa.

-Jag behöver en variabel för en array för att spelet ska ha flera ord att välja ifrån.

-Jag behöver en variabel för fails som låter spelet se hur många gånger man har misslyckats med att gissa rätt ord och sen kunna hänga gubben.

*3; Vilka olika konstrollstrukturer behövs och till vilket syfte? (Loopar, villkor, etc.) Var så detaljerad som möjligt.*

-Jag har en for(loop) och "if" statement som gör så att beroende på hur lång ordet är så lägger den ett "_". "if" statementen gör också att om man gissar rätt ord, dvs om vilkoren ser att bokstavet man har gissat är rätt så lägger den det istället för ett "_", annars fortsätter den som den gjorde.

-Jag har en "if" statement för om man har 6 fails så har man förlorat spelet.


*4; Vilken funktionalitet kan (och borde) du skapa funktioner av? Här vill jag ha funktionsnamn, returtyp, eventuella parametrar samt vad funktionen ska göra.*
-"difficulities" funktion vill jag ha som kollar vilket svårighet spelet ska vara.
-"choose" funktion som väljer ett av de 3 svårighetsgraderna.
-"random" funktion som väljer antingen ett ord eller ett svårighetsgrad som random
-"wordCheck" funktion som tillser om man har gissat rätt ord och hur lång själva ordet är som man ska gissa.

*5; Vilka variabler behöver vara åtkomliga inom hela klassen?*
-Alla, för att spelet behöver veta vilket ord man har, hur många fails man har och hur lång ordet är samt om man har gissat rätt bokstav.
