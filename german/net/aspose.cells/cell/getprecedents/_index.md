---
title: "Cell.GetPrecedents"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt alle Verweise zurück, die in der Formel dieser Zelle vorkommen"
type: docs
url: /de/net/aspose.cells/cell/getprecedents/
---
## Cell.GetPrecedents method

Liefert alle Verweise, die in der Formel dieser Zelle vorkommen.

```csharp
public ReferredAreaCollection GetPrecedents()
```

### Rückgabewert

Sammlung aller Verweise, die in der Formel dieser Zelle vorkommen.

### Hinweise

Gibt null zurück, wenn dies keine Formezelle ist. Alle Verweise, die in der Formel dieser Zelle vorkommen, werden zurückgegeben, unabhängig davon, ob sie bei der Berechnung referenziert werden oder nicht. Zum Beispiel wird die Zelle A2 in der Formel "=IF(TRUE,A1,A2)" zwar nicht bei der Berechnung verwendet, aber dennoch als Vorgänger der Formel betrachtet. Um nur jene Verweise zu erhalten, die die Berechnung beeinflussen, verwenden Sie bitte [`GetPrecedentsInCalculation`](../getprecedentsincalculation/).

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Formel mit Vorgängern festlegen
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1";
            
            // Alle Vorgängerreferenzen abrufen
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Jede Vorgängerreferenz anzeigen
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                if (area.IsArea)
                {
                    sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
                }
                Console.WriteLine(sb.ToString());
            }
        }
    }
}
```

### Siehe auch

* class [ReferredAreaCollection](../../referredareacollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


