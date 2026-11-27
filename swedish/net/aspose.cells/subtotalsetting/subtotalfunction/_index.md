---
title: "SubtotalSetting.SubtotalFunction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SubtotalSetting-egenskap. Subtotal-funktionen"
type: docs
url: /sv/net/aspose.cells/subtotalsetting/subtotalfunction/
---
## SubtotalSetting.SubtotalFunction property

Delssummafunktionen.

```csharp
public ConsolidationFunction SubtotalFunction { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySubtotalFunctionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group A" : "Group B");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Skapa subtotalinställning genom att hämta från befintliga data
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Konfigurera subtotal – dessa egenskaper är skrivskyddade i den faktiska API:n
            // Så använder vi Subtotal-metoden direkt med parametrar
            int groupBy = 0; // Group by first column
            ConsolidationFunction function = ConsolidationFunction.Sum;
            int[] subtotalColumns = new int[] {1}; // Subtotal on second column
            
            // Applicera subtotaler
            worksheet.Cells.Subtotal(area, groupBy, function, subtotalColumns);

            // Verifiera SubtotalFunction-egenskapen från den hämtade inställningen
            Console.WriteLine("Subtotal Function: " + subtotalSetting.SubtotalFunction);
            
            // Spara arbetsboken
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


