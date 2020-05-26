# Closed Captions

Link:

## Gesprek met Darice

Tijdens het gesprek met Darice zijn er een aantal punten besproken waar zij mee te maken krijgt tijdens het kijken van een film. Zo merkt ze bijvoorbeeld dat het soms lastig kan zijn om bij te houden wie er spreekt, vooral als de ondertiteling erg snel gaat. Dit is vooral wanneer er meerdere mensen in de scene aanwezig zijn. Omgevingsgeluiden krijgt ze ook niet mee. Kleur heeft emoties voor Darice, kleur zou je kunnen gebruiken om een gevoel uit te drukken. De kleur zou kunnnen bijdragen aan het overbrengen van een sfeer, zo associeert Darice donkere kleuren met spanning. Voor Darice is het belangrijk dat er consistentie is in de captions. Door de visuele stijl van de tekst, bijvoorbeeld italic, weet Darice van tevoren al waar de captions over gaan puur door de stijl. Door het lezen van captions gaan details soms wel verloren. ALs je de captions leest kan je ondertussen een subtiele verandering in gezichtsuitdrukking missen.

Met deze punten wil ik graag rekening houden tijdens het maken van deze opdracht. Je moet natuurlijk creatief zijn en experimenteren, maar omdat je ook tegelijkertijd voor iemand ontwerpt, wil ik Darice hier bij wel in gedachte houden.


## Fontkeuze Onderbouwing

Ik heb ervoor gekozen om het Brenner font te gebruiken. Brenner bevat veel stijlen en omdat ik graag emotie en sfeer wil overbrengen met mijn captions, leek Brenner mij hiervoor de beste keuze.

**Brenner Sans:** Dit is het "hoofd" font dat ik uiteindelijk heb gekozen. De film speelt zich af in de toekomst. Dit font ziet er modern uit, in tegenstelling tot het reguliere Brenner font die er door de sierlijke uiteindes klassieker uitziet.

**Brenner Sans Bold Italic:** Deze variant heb ik gebruikt om omgevingsgeluiden mee te laten zien. Doordat het font zwaarder is dan de tekst van de dialoog, zijn deze makkelijker te onderscheiden. Hierdoor valt het ongevingsgeluid ook meer op, omdat de letters groot en dik in beeld komen.

**Brenner Sans Regular:** Dit lettertype visualiseert de lopende tekst. Dit is de tekst die je het meest tegenkomt, dus dit moest op een comfortabele manier te lezen zijn. 

**Brenner Mono Regular:** Dit lettertype heb ik toegepast als Officer K's volledige serienummer wordt uitgesproken. Omdat het nummers bevat en op een levenloze mechanise manier wordt uitgesproken, leek dit computer-achtige font mij het meest passend hiervoor.

**Brenner Sans Regular Italic:** Deze gebruik ik voornamelijk voor de spreker. Door het verschil in fontstijl in combinatie met een andere kleur weet je in 1 oogopslag dat er een nieuwe spreker aan bod is.

**Brenner Sans Condensed:** Deze gebruik ik om de aggressie te visualiseren door de politieman aan het begin van het eerste fragment. Het font is een beetje nauw en tegenelkaar gedrukt, net als de manier waarop de belediging van de politieman klinkt. Hij maakt een aggresieve opmerking maar schreeuwt niet naar Officer K, hij houdt zich in.

## Design Principles

## Week 1: Eerste experiment

In de eerste week heb ik een aantal verschillende dingen geprobeerd om te kijken hoe dit door Darice werd ervaren. Ik had een spreker toegevoegd aan de teksten wat het duidelijker zou moeten maken wie er op welk moment aan het woord is. Het contrast mag nog wel wat hoger om de leesbaarheid te bevoorderen. In mijn eerste versie had ik de animaties overeen laten komen met wat er werd gezegd, maar dit kan verwarring veroorzaken. Zo draaide het woord "spin" ook daadwerkelijk rond. Dit kan een misverstand veroorzaken met hoe het woord gezegd word, dus heb ik na de eerste week besloten om mij volledig op de achtergrondgeluiden te focussen. Hieronder zie je een aantal screenshots van mijn eerste versie:

![Week 1](https://user-images.githubusercontent.com/45418246/82219751-00389c00-991e-11ea-98a6-5b5896da268b.png)

## Week 2: Iteraties

In de tweede week heb ik de feedback van de week ervoor doorgevoerd. Zo heb ik meer contrast toegevoegd en heeft de spreker een kleur gekregen zodat je deze bijna onbewust kunt onderscheiden van de dialoog. Daarnaast heb ik het Iframe groter gemaakt en in het midden van de pagina geplaatst. Dit in combinatie met de ondertiteling die nu in de video verschijnt, krijg je meer het bioscoop gevoel. TIjdens dit tweede feedback gesprek kwam naar boven dat Darice graag nog achtergrondgeluiden met tekst ondersteunt wilde zien. Dit maakt het voor haar duidelijker wat voor geluid er precies afspeelt in combinatie met de visuele animaties.

![Week 2](https://user-images.githubusercontent.com/45418246/82929428-eaf9e800-9f83-11ea-8f7a-cd7e38fc3fec.png)

## Week 3: Eindproduct

Hieronder wordt per belangrijke animatie uitgelegd wat ik heb gedaan.

**Openingsscene**

In de openingsscene komt Officer K aangevlogen in een voertuig. Door het Iframe te laten schudden met `transform: Rotate(xdeg)` Heb ik geprobeerd het rommelende geluid en de lichte vibratie in het voertuig te laten zien. Het moment waar Offcier K's serienummer wordt opgeroepen, verschijnen de nummers 1 voor 1 om de mechanische toon van de stem te versterken. Dit heb ik gedaan door op elk nummer een `transition` te zetten.

![Openingsscene](https://user-images.githubusercontent.com/45418246/82931464-41b4f100-9f87-11ea-925c-a7c6fca7f20c.gif)


**Alarm**

In de 2 fragmenten zijn 3 soorten alarmen en sirenes te vinden. Het eerste alarm is hard en schel, deze eindigt abrupter dan de andere alarmen. Het scherm wordt snel even rood en is dan weer zwart. Een sirene gaat af. Het harder en zachter worden van de sirene laat ik zien door de kleuren wit en rood elkaar te laten afwisselen. Het derde alarm, een soort luide mechanische piep, schuift in de achtergrond langs. Het alarm "rolt" als het ware over de achtergrond. Tijdens het fragment zijn er soms geluiden die vanuit een specifieke locatie komen; dit zie je hier aan de "voice through microphone". Deze is op het scherm op het gebouw geplaatst om aan te duiden waar het vandaan komt. 

Ik heb de geluiden en de teksten tegelijk kunnen laten afspelen door `::Before` en `::after` te gebruiken en `content` toe te voegen aan de `class` die op dat moment op de `body` verschijnt. Het alarm heb ik gemaakt door een `linear-gradient` op de achtergrond te zetten waarvan de `background-position`veranderd.

![Alarmen](https://user-images.githubusercontent.com/45418246/82932545-e257e080-9f88-11ea-8588-bb54d4b48094.gif)

![Specifiek geluid](https://user-images.githubusercontent.com/45418246/82932994-948fa800-9f89-11ea-98bd-4b1450c0394b.gif)


**Aggressie**

Om duidelijk te maken dat de politieman een gemene opmerking maakt heb ik de tekst rood gemaakt en laten trillen. Het font heb ik niet al te groot gemaakt; ik wil niet laten lijken alsof hij schreeuwt. Dit trillen heb ik met `transform: Skew (xdeg)` gedaan en vervolgens snel laten afspelen om de trilling te veroorzaken.

![Aggressie](https://user-images.githubusercontent.com/45418246/82936396-d1aa6900-9f8e-11ea-867d-922e483a8f5c.gif)

**Baseline test 1**

Tijdens deze scene klinkt er een hoge toon die alsmaar luider wordt. Dit heb ik gevisualiseerd met de achtergrond die steeds feller en lichter wordt. Daarnaast verschijnt de omschrijvende tekst steeds groter in beeld. Aan het einde van de scene wanneer de hoge toon stopt, wordt de achtergrond weer donker en verdwijnt de omschrijvende tekst om aan te geven dat het geluid voorbij is. Dit heb ik gedaan door `keyframes` aan te maken met percentages, waarbij 100% de witte kleur is. Door een afspeeltijd in seconden mee te geven aan de `animation` speelt deze af gedurende de hoge toon.

De captions wisselen elkaar af. Korte zinnen van de Questioner verschijnen links, terwijl Officer K zijn tekst rechts verschijnt. Hiermee wil ik de snelle afwisseling van de dialoog visualiseren en ook die mechanische sfeer overbrengen. Het is alsof 2 robots tegen elkaar praten. Dit heb ik gedaan door een aantal `marges` mee te geven aan de gesproken tekst.

![Baseline test 1](https://user-images.githubusercontent.com/45418246/82937580-ae80b900-9f90-11ea-8320-d29c69570fed.gif)

**Muziek**

Tijdens de tweede Baseline test klinkt er muziek op de achtergrond. Deze heb ik gevisualiseerd met een pulserende gradient die donker en licht wordt samen met de muziek die hard en zacht klinkt. De muziek verloopt als een soort golf, daarom heb ik ook een geanimeerde gradient gebruikt.

![Muziek](https://user-images.githubusercontent.com/45418246/82945539-66b45e80-9f9d-11ea-8510-dee5e7cdb68f.gif)

**Vertraging**

Op een gegeven moment lijkt het alsof de Questioner langzamer praat. Omdat dit normaal in lopende tekst verloren gaat heb ik hier een `delay` gezet op de individuele woorden. Ook heb ik de stijl van de woorden aangepast om te laten zien dat op dit moment de stem anders klinkt dan normaal en vertraagd lijkt.

![Vertraging](https://user-images.githubusercontent.com/45418246/82946037-f0fcc280-9f9d-11ea-9b3e-efc45962334d.gif)


**Twijfel**

Officer K lijkt in de tweede Baseline test minder zeker van zijn zaak. Zijn antwoorden zijn minder mechanisch en hij lijkt op momenten een soort twijfel te vertonen. Daarom heb ik in de `html` "..." toegevoegd, om zo ook via tekst over te brengen dat er iets is veranderd in Officer K.

![Twijfel](https://user-images.githubusercontent.com/45418246/82946390-8ef08d00-9f9e-11ea-9456-799101001a09.gif)
