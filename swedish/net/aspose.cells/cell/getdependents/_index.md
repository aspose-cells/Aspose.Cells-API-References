---
title: GetDependents
second_title: Aspose.Cells för .NET API-referens
description: Få alla celler vars formel refererar till den här cellen direkt.
type: docs
weight: 380
url: /sv/net/aspose.cells/cell/getdependents/
---
## Cell.GetDependents method

Få alla celler vars formel refererar till den här cellen direkt.

```csharp
public Cell[] GetDependents(bool isAll)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isAll | Boolean | Anger om kontrollera formler i andra kalkylblad |

### Anmärkningar

Om en referens som innehåller den här cellen visas i en cells formel, kommer den cellen att tas som beroende av denna cell, oavsett referensen eller denna cell används eller inte under beräkningen. Till exempel, även om cell A2 i formeln "=IF (TRUE,A1,A2)" används inte vid beräkning, denna formel är fortfarande beroende av A2.  För att få de formler vars beräknade resultat beror på denna cell, använd[`GetDependentsInCalculation`](../getdependentsincalculation). När du spårar beroende för en cell kommer alla formler i arbetsboken eller kalkylbladet att analyseras och kontrolleras. Så det är en tidskrävande process. Om användaren behöver spåra anhöriga för många celler, kommer den här metoden att orsaka dålig prestanda. För prestandaövervägande bör användaren använda[`GetDependentsInCalculation`](../getdependentsincalculation) istället. Eller så kan användaren samla prejudikatkarta över alla celler genom[`GetPrecedents`](../getprecedents)först, och sedan bygga den beroende kartan enligt prejudikatkartan.

### Exempel

```csharp
[C#]

Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
cells["A2"].Formula = "=IF(TRUE,B2,B1)";
Cell[] dependents = cells["B1"].GetDependents(true);
for (int i = 0; i < dependents.Length; i++)
{
     Console.WriteLine(dependents[i].Name);
}
```

### Se även

* class [Cell](../../cell)
* namnutrymme [Aspose.Cells](../../cell)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
