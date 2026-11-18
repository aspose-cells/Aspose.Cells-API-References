---
title: "CalculationOptions klass"
linktitle: "CalculationOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "CalculationOptions klass. Inkapslar objektet som representerar calculationoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/calculationoptions/
---

## CalculationOptions class

Representerar alternativ för beräkning.

```go

type CalculationOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewCalculationOptions](./newcalculationoptions/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetIgnoreError](./getignoreerror/) | Anger om fel som uppstår vid beräkning av formler ska ignoreras.Fel kan vara en funktion som inte stöds, externa länkar osv.Det förvalda värdet är sant. |
| [SetIgnoreError](./setignoreerror/) | Anger om fel som uppstår vid beräkning av formler ska ignoreras.Fel kan vara en funktion som inte stöds, externa länkar osv.Det förvalda värdet är sant. |
| [GetRecursive](./getrecursive/) | Anger om de beroende cellerna ska beräknas rekursivt när en cell beräknas och den beror på andra celler.Det förvalda värdet är sant. |
| [SetRecursive](./setrecursive/) | Anger om de beroende cellerna ska beräknas rekursivt när en cell beräknas och den beror på andra celler.Det förvalda värdet är sant. |
| [GetUserSpecifiedRefreshDynamicArrayFormula](./getuserspecifiedrefreshdynamicarrayformula/) | Anger om användaren uttryckligen har specificerat beteendet för att uppdatera dynamiska arrayformler innan angivna formler beräknas. |
| [GetRefreshDynamicArrayFormula](./getrefreshdynamicarrayformula/) | Anger om dynamiska arrayformler ska uppdateras innan formler beräknas. |
| [SetRefreshDynamicArrayFormula](./setrefreshdynamicarrayformula/) | Anger om dynamiska arrayformler ska uppdateras innan formler beräknas. |
| [GetCustomEngine](./getcustomengine/) | Den anpassade formelberäkningsmotorn för att utöka standardberäkningsmotorn i Aspose.Cells. |
| [SetCustomEngine](./setcustomengine/) | Den anpassade formelberäkningsmotorn för att utöka standardberäkningsmotorn i Aspose.Cells. |
| [GetCalcStackSize](./getcalcstacksize/) | Stackstorleken för rekursiv beräkning av celler. Standardvärdet är 200. |
| [SetCalcStackSize](./setcalcstacksize/) | Stackstorleken för rekursiv beräkning av celler. Standardvärdet är 200. |
| [GetPrecisionStrategy](./getprecisionstrategy/) | Anger strategin för bearbetning av beräkningsprecision. |
| [SetPrecisionStrategy](./setprecisionstrategy/) | Anger strategin för bearbetning av beräkningsprecision. |
| [GetLinkedDataSources](./getlinkeddatasources/) | Anger datakällorna för externa länkar som används i formler. |
| [SetLinkedDataSources](./setlinkeddatasources/) | Anger datakällorna för externa länkar som används i formler. |
| [GetCharacterEncoding](./getcharacterencoding/) | Anger den kodning som används för kodning/avkodning av tecken vid beräkning av formler. För funktioner såsom CHAR, CODE beror det beräknade resultatet på regionsinställningarna och standardteckenuppsättningen i miljön. Med den här egenskapen kan användaren ange rätt kodning som används för dessa funktioner för att få det förväntade resultatet. |
| [SetCharacterEncoding](./setcharacterencoding/) | Anger den kodning som används för kodning/avkodning av tecken vid beräkning av formler. För funktioner såsom CHAR, CODE beror det beräknade resultatet på regionsinställningarna och standardteckenuppsättningen i miljön. Med den här egenskapen kan användaren ange rätt kodning som används för dessa funktioner för att få det förväntade resultatet. |
