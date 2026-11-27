---
title: "PivotTable.AltTextTitle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar och anger titeln för den alternativa texten"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/alttexttitle/
---
## PivotTable.AltTextTitle property

Hämtar och anger titeln för den alternativa texten.

```csharp
public string AltTextTitle { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyAltTextTitleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);

            // Skapa en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "SalesPivotTable");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa aktuellt AltTextTitle‑värde
            Console.WriteLine("Current AltTextTitle value: " + pivotTable.AltTextTitle);

            // Ange nytt AltTextTitle‑värde
            pivotTable.AltTextTitle = "Sales Data Pivot Table";

            // Beräkna pivottabellsdata
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableAltTextTitleDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


