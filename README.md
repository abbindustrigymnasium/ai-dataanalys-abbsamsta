# Cardifier AI 

## Innehållsförteckning 

- [Målet](#målet)
  - [Detta projekt](#detta-projekt)
  - [Vidarutveckling](#vidarutveckling)
- [Uppbyggnad](#uppbyggnad)
  - [OpenCV](#opencv)
  - [YOLO](#yolo)
  - [Google Collab](#google-collab)
- [Resultat](#resultat)
- [Problem och lärdom](#problem-och-lärdom)
  - [Hitta en massa bilder](#hitta-en-massa-bilder)
  - [Installera alla dependencies](#installera-alla-dependencies)
  - [Brist på kunskap under tidspressen](#brist-på-kunskap-under-tidspressen)

# Målet

## Detta projekt
Målet med detta projekt var att bygga en AI som kan identifiera vilken bilmodel som finns på kameran. Det preliminära målet var främst att AI:n skulle kunna känna igen om det var huven av en Volvo V40 eller V90 som befann sig på bilden. Detta systen skulle sedan vidarutvecklas till att kunna känna igen fler modeller av Volvo och slutligen olika bilmärken.

- Cardifier 1.0 - Identifiera om det är huven av en Volvo V40 eller V90 som visas
- Cardifier 2.0 - Identifiera vilken del av bilen som helst
- Cardifier 3.0 - Identifiera vilken Volvo-modell som helst
- Cardifier 4.0 - Identifiera alla möjliga bilmärken

## Vidarutveckling
Den framtida vision som finns med projektet att kommer fungera som ett bibliotek för andra utvecklare att bygga vidare på. Ett exempel är att skapa en mobilapplikation som först använder sig av Cardifier AI för att identifiera bilmodellen och sedan visar specifikationer om den.

# Uppbyggnad
Som hjälp för att utveckla Cardifier användes 

### OpenCV
OpenCV är grunden för att jobba med bilder i Python.

### YOLO
Yolo är det verktyg för OpenCV som är tänkt att användas för att finna objekt (d.v.s bilen i dett fall) i allt ifrån bild, video och direkt ifrån en kamera.

### Google Collab
Googles Collab program används sedan för att träna YOLO-programmet. Collab låter Yolo träna på molnet istället för lokalt på datorn. Det gör att jag kan komma åt träningen från både skoldatorn och hemdatorn.

# Resultat
Utav detta projekt har jag lärt mig mycket om ämnet "Computer Vision". Jag har fått exprimentera med roliga verktyg såsom OpenCV, YOLO och Google Collab.

# Problem och lärdom
Under vägens gång stötte jag  på en hel del tidskrävande problem, dock var de inga svåra problem att lösa. Utifrån detta hoppas jag kunna ta med mig av en hel del värdigfull erfarenhet inför framtida projekt.

### Hitta en massa bilder

Anledningen till att Cardifier 1.0 bara var tänkt att innehålla identifiering av Volvo V40 och V90 är för att det var klart för mig redan innan att det kommer ta lång tid att sammla bra meterial för AI:n att träna med. Därför valdes ett begränsat antal bilar för att minimera tiden för onödigt bildletande. 

Att hitta rätt bilder som är bra för AI:n att träna med tar en hel del tid att hitta och det spendera lite för mycket tid till att hitta de bilder som behövdes. 

### Installera alla dependencies
Under intallationen allt material som behövdes för detta tog längre tid en väntat och skpade en hel del huvudvärk. Under processen kunde jag få upp skumma problem som: "Du kan inte uppdatera PiP för att du har en för gammal uppdatering av PiP." De var sällan svåra att lösa men de tog onödigt mycket tid.

![PiP](https://github.com/abbindustrigymnasium/ai-dataanalys-abbsamsta/blob/master/Presentation/bild1.png)

Ett annat exempel är hur cv2 inte ville installera för de "kunde inte hitta en uppdatering som matchade med dess egna krav" när jag skrev inte "pip install cv2"...

![cv2](https://github.com/abbindustrigymnasium/ai-dataanalys-abbsamsta/blob/master/Presentation/bild2.png)

### Brist på kunskap under tidspressen

Att skapa en AI på 10h är nog inget svårt egentligen. Problemet i detta projekt blev att jag kunde för lite om specifikt "image recognition" när jag startade projektet vilket gjorde att jag behövde lägga lite väl mycket tid på att faktiskt förstå mig på OpenCV, YOLO och Google Collab innan jag kunde börja jobba. Detta positiva nu är väll att jag åtminstone lärt mig det och skulle kunna färdigställa projeketet med lite extra tid.

