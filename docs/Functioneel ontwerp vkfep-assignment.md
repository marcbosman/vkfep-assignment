# Hardware uitleen app

Functioneel ontwerp

# Inhoudsopgave

1. [ Inleiding ](#inleiding)
2. [ State diagrams ](#statediag)
3. [ Use case diagram ](#ucdiag)
4. [ Use case summaries ](#ucsum)

<a name="inleiding"></a>
# 01. Inleiding

TODO

<a name="statediag"></a>
# 02. State diagrams

![State diagram Hardware uitleen app](./State_Diagram.png)

<a name="ucdiag"></a>
# 03. Use Case diagram

![Use case diagram Hardware uitleen app](./Use_Case_Diagram.png)

<a name="ucsum"></a>
# 04. Use case summaries

Actor               | Use Case                              | Samenvatting
------------------- | ------------------------------------- | ----
Student             | Product lenen                         | De student kan alleen producten lenen met de status "Beschikbaar", of, als het product de status "Gereserveerd" heeft en het emailadres van de student bij het gereserveerde product staat. Als een student een product heeft gekozen om te lenen, krijgt dit product de status "Uitgeleend". <br>Het systeem genereerd een uiterste inleverdatum voor het product op basis van het huidige schoolblok. De uiterste inleverdatum zal dan gelijk staan aan het einde van de laatste dag van het huidige schoolblok. Het systeem voert ook automatisch het email adres van de ingelogde student in.
Student             | Product reserveren                    | Als een product al reeds de status "Uitgeleend" heeft, of als de student het product in het aankomende blok wil gebruiken, kan de student er voor kiezen om het product te reserveren. Het systeem wijst dan een reserveringsdatum toe aan het product. <br>Als het product nog de status "Beschikbaar" heeft, zal de reserveringsdatum gelijk staan aan de huidige dag. Als het product de status "Uitgeleend" heeft, zal de reserveringsdatum gelijk staan aan het begin van de eerste dag van het aankomende schoolblok. In beide gevallen zal het systeem het email van de student koppelen aan het product.
Student, Beheerder  | Overzicht van producten inzien        | De genoemde actoren moeten een overzicht van toegevoegde producten (out) kunnen inzien met per product de __titel__, de __details__, een __fotoimpressie__ en de __status__ van het product (beschikbaar, uitgeleend, gereserveerd, defect) (out). De student heeft hier de mogelijkheid om een product te lenen. De beheerder heeft hier de mogelijkheid om producten toe te voegen, te verwijderen en aan te passen.
Beheerder           | Product toevoegen                     | De beheerder kan een product toevoegen door in het overzicht van producten op de knop "product toevoegen" te klikken en in het hieropvolgende scherm een __titel__, de __details__ en een __foto__ toe te voegen (in). 
Beheerder           | Product verwijderen                   | De beheerder kan een product verwijderen door in het overzicht van producten het __product__ te selecteren en op "product verwijderen" te klikken (in).
Beheerder           | Product aanpassen                     | De beheerder kan een product aanpassen door in het overzicht van producten of in het detailscherm van een product op de knop "product aanpassen" te klikken en in het hieropvolgende scherm de __titel__, __details__ en/of __foto__ aan te passen (in). 
Beheerder           | Product aangeven als geleend          | De beheerder kan een product aangeven als geleend door het __product__ te selecteren, hier een __student__ aan toe te wijzen en de __duur van de lening__ in te stellen (in).
Beheerder           | Product aangeven als beschikbaar      | todo
Beheerder           | Lijst van te late inleveringen inzien | Een product dat te laat is ingeleverd is gedefinieerd als een product met status "Uitgeleend", waarbij de uiterste inleverdatum kleiner (eerder) is als de huidige datum. De beheerder kan van het systeem een lijst opvragen met alle te laat ingeleverde producten. Hierbij geeft het systeem per product de uiterste inleverdatum en het emailadres van de student die het product heeft geleend.

