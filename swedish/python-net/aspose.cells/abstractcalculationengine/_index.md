---
title: AbstractCalculationEngine klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/abstractcalculationengine/
is_root: false
---
##  AbstractCalculationEngine klass
Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn Aspose.Cells.



Typen AbstractCalculationEngine avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [is_param_literal_required](/cells/sv/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required) | Indikerar om denna motor behöver den bokstavliga texten i parametern när den gör beräkning. Standardvärdet är falskt.|
| [process_built_in_functions](/cells/sv/python-net/aspose.cells/abstractcalculationengine/process_built_in_functions) | Huruvida inbyggda funktioner som har stöds av den inbyggda motorn bör kontrolleras och bearbetas av denna implementering.<br/>Standard är falskt.<br/> Om användaren behöver ändra beräkningslogiken för vissa inbyggda funktioner, ska denna egenskap ställas in som true.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [calculate(data)](/cells/sv/python-net/aspose.cells/abstractcalculationengine/calculate/#CalculationData) | Beräknar en funktion med givna data.|



###  Anmärkningar

Användaren bör inte ändra någon del av arbetsboken direkt i den här implementeringen (förutom det beräknade resultatet av den anpassade funktionen, som kan ställas in av egenskapen CalculationData.CalculatedValue).
Annars kan oväntade resultat eller undantag orsakas.
Om användaren behöver ändra andra data än det beräknade resultatet i implementeringen av vissa anpassade funktioner,
till exempel ändra cells formel, stil, ... etc., användaren ska samla in dessa data i den här implementeringen och ändra dem utanför ramen för formelberäkningen.

###  Se även
* modul [aspose.cells](..)
