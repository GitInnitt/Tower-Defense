Sprint 0 - Game Design Document : Tower Defense
Naam: Sam

Klas: SD2A

Datum: 8/9/2025

1. Titel en elevator pitch
Titel: Marvel Defense

Elevator pitch, maximaal twee zinnen: 

Een tower defense game met Marvel characters. Versla villains van de Marvel universe om coins te krijgen en sterke heroes te kopen. Om de abillities te doen moet je abillity fluid uitgeven. Elke wave krijg je er 2 en je kan max 20 abillity fluid bij je houden.

2. Wat maakt jouw tower defense uniek
   
Je speelt met en tegen iconische Marvel heroes in een tower defense game op Marvel themed maps. Tower troop combo's geven toegang tot speciale abillities

3. Schets van je level en UI
Maak een schets op papier of digitaal en voeg deze afbeelding toe aan je repository. Voeg in deze sectie de afbeelding in.
<img width="1162" height="673" alt="Tekening Game (Nieuw en goed)" src="https://github.com/user-attachments/assets/7bb1c1c1-7f41-476e-b502-fdbabb406dbd" />


4. Torens
   
Toren 1 naam: Front, bereik: ?, schade: begint bij 1 (wordt sterker na upgrades), unieke eigenschap.

Toren 2 naam: Mid 1, bereik: ?, schade: begint bij 1 (wordt sterker na upgrades), unieke eigenschap.

Toren 3 naam: Mid 2, bereik: ?, schade: begint bij 1 (wordt sterker na upgrades), unieke eigenschap.

Toren 4 naam: Back, bereik: ?, schade: begint bij 1 (wordt sterker na upgrades), unieke eigenschap.

5. Vijanden
   
Vijand 1 naam: Melee, snelheid: 1, levens: 10 (2 extra levens per wave), damage: 3, speciale eigenschap: N.V.T., Gold per kill: 2.

Vijand 2 naam: Ranger, snelheid: 1, levens: 7 (2 extra levens per wave), damage: 2, speciale eigenschap: Schiet op afstand op towers met bommen, waardoor de tower kort gestunned worden., Gold per kill: 3

Vijand 3 naam: Tank, snelheid: 0.5, levens: 15 (2 extra levens per wave), damage: 5, speciale eigenschap: Is sterker dan normale zombies maar lopen wat slomer, Gold per kill: 6

Vijand 4 naam: Speedster, snelheid: 3, levens: 7 (2 extra levens per wave), damage: 3, speciale eigenschap: Is sneller dan normale enemies, Gold per kill: 3

6. Gameplay loop

-Schiet enemies

-Krijg coins voor enemies killen

-Spendeer de coins in de shop voor upgrades

-Haal een zo hoog mogelijke high score

-unlock alle characters

7. Progressie
Leg uit hoe het spel moeilijker wordt naarmate de waves doorgaan. Denk aan sterkere vijanden, kortere tussenpozen, hogere kosten of lagere beloningen.

Elke wave krijgt elke enemy 2 levens extra en spawnen er meer enemies. Betere heroes gaan steeds meer coins kosten en betere team ups gaan meer abillity fluid kosten.

8. Risico’s en oplossingen volgens PIO
    
Probleem 1: Enemies volgen pad niet.

Impact: De enemies lopen niet hoe ze horen te lopen

Oplossing: Een script maken die dat voorkomt

Probleem 2: Towers schieten niet goed.

Impact: De game is onspeelbaar

Oplossing: Code maken zodat ze de enemies goed schieten

Probleem 3: Abillities kunnen niet ingezet worden

Impact: Game wordt veel moeilijker

Oplossing: De knop maken hoe je het kan inzetten

9. Planning per sprint en mechanics
Schrijf per sprint welke mechanics jij oplevert in de build. Denk aan voorbeelden zoals vijandbeweging over een pad, torens plaatsen, doel kiezen en schieten, waves starten, UI voor geld en levens, upgrades, jouw unieke feature.

Sprint 1 mechanics: Core game maken, (Towers die schieten, enemies die het pad volgen)

Sprint 2 mechanics: Extra mechanics maken, (Gold counter die omhoog gaat, Pauze knop, Wave system en Lives system)

Sprint 3 mechanics: Extra mechanics afmaken en shop maken voor upgrades

Sprint 4 mechanics: Abillity Fluid laten werken

Sprint 5 mechanics: Laatste checks zodat alles werkt, mogelijk updates voor bestaande mechanics maken

10. Inspiratie

Heb geen specifieke tower defense game waar ik inspiratie van haal maar verschillende andere games

-Marvel Rivals - Characters en enemies

-Clash Royale - Abillity Fluid

11. Technisch ontwerp mini
Lees dit korte voorbeeld en vul daarna jouw eigen keuzes in.
(Maak deze later)

11.1 Vijandbeweging over het pad

Keuze: De enemy waypoints laten volgen tot de eindbestemming.

Risico: Vijanden lopen niet goed over het pad of slaan 1 checkpoint over waar ze naartoe zouden moeten lopen.

Oplossing: Ervoor zorgen in de code dat dit soort problemen opgelost worden en voorkomen worden.

Acceptatie: De enemy moet altijd het pad blijven volgen zodat de game goed en eerlijk blijft werken.

11.2 Doel kiezen en schieten

Keuze: De towers moeten constant op de dichtsbijzijnde enemy schieten zodat de enemies niet te snel of dat er rng ontstaat omdat de sterkere enemies als eerst gekilled worden.

Risico: Dat de torens compleet random op enemies schieten waardoor er een deel rng ontstaat in de game.

Oplossing: een stukje toevoegen aan het script dat de dichtsbijzijnde enemy als eerst geschoten wordt.

Acceptatie: Dat de dichtsbijzijnde enemy als eerst geschoten wordt zorgt ervoor dat er geen soort rng is in de game waardoor het niet randomness is.

11.3 Waves en spawnen

Keuze: Elke ronde komen er 2-3 zombies bij en dat wordt elke 10 waves verdubbeld.

Risico: Dat enemies niet goed spawnen of helemaal niet spawnen.

Oplossing: Een script maken waardoor er telkens 2-3 enemies bijkomen per wave en wat uiteindelijk verdubbeld wordt.

Acceptatie: Dat naar mate je langer in de game zit hoe moeilijker de waves worden waardoor je het uiteindelijk enorm lastig zult gaan krijgen.

11.4 Economie en levens

Keuze: Je hoofdtoren heeft bij start 1000 HP die vermindert door enemy attacks. Per enemy die je killed krijg je gold om nieuwe heroes te kopen wat per 5 waves meer wordt.

Risico: HP van de toren gaat niet omlaag of gold wordt niet getelt bij de kill van een enemy.

Oplossing: Ervoor zorgen dat je een script hebt die aftelt vanaf 1000 per keer dat een enemy de laatste checkpoint bereikt en een script maken dat er gold opgetelt wordt elke keer als je een enemy killed.

Acceptatie: Dat je veel enemies moet gaan killen om een betere defense te krijgen en je gold slim moet uitgeven voor de beste upgrades.

11.5 UI basis

Keuze: Aan de linkerkant van het scherm zit een knopje om de shop te openen waar je heroes kunt kopen. Aan de rechterkant staan o.a. Je levens, Abillity fluid en Gold

Risico: De shop opent niet als je op de knop klikt waardoor je geen nieuwe/betere defenses kunt kopen wat ervoor zorgt dat je heel snel af gaat

Oplossing: Code schrijven dat de shop normaal opent zonder visual glitches zodat je makkelijk de heroes kunt kopen en kunt gebruiken op het speelveld.

Acceptatie: De UI wordt duidelijk en makkelijk te volgen zodat je alles makkelijk kan zien wat belangrijk is in de UI.
