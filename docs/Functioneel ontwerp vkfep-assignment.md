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
Student             | Product lenen                         | todo
Student             | Product reserveren                    | todo
Student, Beheerder  | Overzicht van producten inzien        | De genoemde actoren moeten een overzicht van toegevoegde producten (out) kunnen inzien met per product de __titel__, de __details__, een __fotoimpressie__ en de __status__ van het product (beschikbaar, uitgeleend, gereserveerd, defect) (out). De student heeft hier de mogelijkheid om een product te lenen. De beheerder heeft hier de mogelijkheid om producten toe te voegen, te verwijderen en aan te passen.
Beheerder           | Product toevoegen                     | De beheerder kan een product toevoegen door in het overzicht van producten op de knop "product toevoegen" te klikken en in het hieropvolgende scherm een __titel__, de __details__ en een __foto__ toe te voegen (in). 
Beheerder           | Product verwijderen                   | De beheerder kan een product verwijderen door in het overzicht van producten het __product__ te selecteren en op "product verwijderen" te klikken (in).
Beheerder           | Product aanpassen                     | De beheerder kan een product aanpassen door in het overzicht van producten of in het detailscherm van een product op de knop "product aanpassen" te klikken en in het hieropvolgende scherm de __titel__, __details__ en/of __foto__ aan te passen (in). 
Beheerder           | Product aangeven als geleend          | De beheerder kan een product aangeven als geleend door het __product__ te selecteren, hier een __student__ aan toe te wijzen en de __duur van de lening__ in te stellen (in).
Beheerder           | Product aangeven als beschikbaar      | todo
Beheerder           | Lijst van te late inleveringen inzien | todo
