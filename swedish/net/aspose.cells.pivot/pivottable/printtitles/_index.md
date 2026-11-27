---
title: "PivotTable.PrintTitles"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om utskriftsrubrikerna för kalkylbladet är inställda baserat på PivotTable-rapporten. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/printtitles/
---
## PivotTable.PrintTitles property

Anger om utskriftsrubrikerna för kalkylbladet sätts baserat på PivotTable‑rapporten. Standardvärdet är false.

```csharp
public bool PrintTitles { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPrintTitlesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och lite exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Konfigurera pivottabellens fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Demonstrera PrintTitles-egenskapen
            pivotTable.PrintTitles = true;
            Console.WriteLine("PrintTitles set to: " + pivotTable.PrintTitles);

            // Spara arbetsboken
            workbook.Save("PivotTablePrintTitlesDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


