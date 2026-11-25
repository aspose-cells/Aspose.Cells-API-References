---
title: "ReferredArea.EndRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReferredArea. La riga finale dell'area"
type: docs
url: /it/net/aspose.cells/referredarea/endrow/
---
## ReferredArea.EndRow property

La riga finale dell'area.

```csharp
public int EndRow { get; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyEndRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Imposta la formula con riferimenti multipli
            cells["A1"].Formula = "= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1";
            
            // Ottieni tutte le aree precedenti
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Elabora ogni riferimento
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                
                // Dimostra l'uso di EndRow per i riferimenti di intervallo
                if (area.IsArea)
                {
                    sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
                }
                
                Console.WriteLine(sb.ToString());
            }
            
            workbook.Save("ReferredAreaExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


