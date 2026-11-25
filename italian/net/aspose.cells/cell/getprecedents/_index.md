---
title: "Cell.GetPrecedents"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottiene tutti i riferimenti presenti nella formula di questa cella"
type: docs
url: /it/net/aspose.cells/cell/getprecedents/
---
## Cell.GetPrecedents method

Ottiene tutti i riferimenti presenti nella formula di questa cella.

```csharp
public ReferredAreaCollection GetPrecedents()
```

### Valore di ritorno

Raccolta di tutti i riferimenti presenti nella formula di questa cella.

### Osservazioni

Restituisce null se questa non è una cella di formula. Tutti i riferimenti presenti nella formula di questa cella verranno restituiti indipendentemente dal fatto che siano referenziati o meno durante il calcolo. Ad esempio, sebbene la cella A2 nella formula "=IF(TRUE,A1,A2)" non sia utilizzata durante il calcolo, viene comunque considerata come precedente della formula. Per ottenere solo i riferimenti che influenzano il calcolo, si prega di utilizzare [`GetPrecedentsInCalculation`](../getprecedentsincalculation/).

### Esempi

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
            
            // Imposta la formula con i precedenti
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1";
            
            // Ottieni tutti i riferimenti precedenti
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Visualizza ogni riferimento precedente
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

### Vedi anche

* class [ReferredAreaCollection](../../referredareacollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


