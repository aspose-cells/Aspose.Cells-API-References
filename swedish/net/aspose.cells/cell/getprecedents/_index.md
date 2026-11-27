---
title: "Cell.GetPrecedents"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cellmetod. Hämtar alla referenser som förekommer i den här cellens formel"
type: docs
url: /sv/net/aspose.cells/cell/getprecedents/
---
## Cell.GetPrecedents method

Hämtar alla referenser som förekommer i cellens formel.

```csharp
public ReferredAreaCollection GetPrecedents()
```

### Returvärde

Samling av alla referenser som förekommer i den här cellens formel.

### Anmärkningar

Returnerar null om detta inte är en formelcell. Alla referenser som förekommer i den här cellens formel kommer att returneras oavsett om de refereras eller inte under beräkningen. Till exempel, även om cell A2 i formeln "=IF(TRUE,A1,A2)" inte används vid beräkning, tas den fortfarande som formelns föregångare. För att endast få de referenser som påverkar beräkningen, använd [`GetPrecedentsInCalculation`](../getprecedentsincalculation/).

### Exempel

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
            
            // Ange formel med föregångare
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1";
            
            // Hämta alla föregångarreferenser
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Visa varje föregångarreferens
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

### Se även

* class [ReferredAreaCollection](../../referredareacollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


