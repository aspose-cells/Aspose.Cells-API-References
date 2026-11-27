---
title: "PivotTable.ShowEmptyRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om tomma rader ska inkluderas i tabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showemptyrow/
---
## PivotTable.ShowEmptyRow property

Anger om tomma rader ska inkluderas i tabellen.

```csharp
public bool ShowEmptyRow { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med några tomma rader
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["B2"].Value = "TV";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Electronics";
            worksheet.Cells["B3"].Value = "";
            worksheet.Cells["C3"].Value = "";
            
            worksheet.Cells["A4"].Value = "Furniture";
            worksheet.Cells["B4"].Value = "Chair";
            worksheet.Cells["C4"].Value = 500;
            
            worksheet.Cells["A5"].Value = "Furniture";
            worksheet.Cells["B5"].Value = "";
            worksheet.Cells["C5"].Value = "";

            // Skapa en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa aktuellt värde för ShowEmptyRow
            Console.WriteLine("Initial ShowEmptyRow value: " + pivotTable.ShowEmptyRow);

            // Visa tomma rader i pivottabellen
            pivotTable.ShowEmptyRow = true;
            Console.WriteLine("ShowEmptyRow set to: " + pivotTable.ShowEmptyRow);

            // Beräkna data för att fylla pivottabellen
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableShowEmptyRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


