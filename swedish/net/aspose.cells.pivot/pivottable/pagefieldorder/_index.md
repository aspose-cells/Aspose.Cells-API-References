---
title: "PivotTable.PageFieldOrder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar och anger ordningen i vilken sidfält läggs till i PivotTable-rapportens layout"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/pagefieldorder/
---
## PivotTable.PageFieldOrder property

Hämtar och anger ordningen i vilken sidfält läggs till i PivotTable‑rapportens layout.

```csharp
public PrintOrderType PageFieldOrder { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldOrderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Region";
            cells["D1"].Value = "Sales";
            
            // Lägg till rader med exempeldata
            for (int i = 2; i <= 10; i++)
            {
                cells[$"A{i}"].Value = $"Category{(i % 3) + 1}";
                cells[$"B{i}"].Value = $"Product{(i % 4) + 1}";
                cells[$"C{i}"].Value = $"Region{(i % 2) + 1}";
                cells[$"D{i}"].Value = i * 100;
            }

            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:D11", "F5", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till fält i områden
            pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Category"]);
            pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Region"]);
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Product"]);
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);

            // Ställ in sidfältets ordning och radbrytningsantal
            pivotTable.PageFieldOrder = PrintOrderType.DownThenOver;
            pivotTable.PageFieldWrapCount = 2;

            // Spara arbetsboken
            workbook.Save("PivotTablePageFieldOrderDemo_out.xlsx");
        }
    }
}
```

### Se även

* enum [PrintOrderType](../../../aspose.cells/printordertype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


