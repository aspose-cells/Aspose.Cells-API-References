---
title: "PivotTable.FieldListSortAscending"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om fält i PivotTable sorteras i icke-standardordning i fältlistan"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/fieldlistsortascending/
---
## PivotTable.FieldListSortAscending property

Anger om fält i pivottabellen sorteras i en icke‑standardordning i fältlistan.

```csharp
public bool FieldListSortAscending { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyFieldListSortAscendingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["B2"].Value = "Laptop";
            worksheet.Cells["C2"].Value = 1200;
            
            worksheet.Cells["A3"].Value = "Electronics";
            worksheet.Cells["B3"].Value = "Phone";
            worksheet.Cells["C3"].Value = 800;
            
            worksheet.Cells["A4"].Value = "Furniture";
            worksheet.Cells["B4"].Value = "Chair";
            worksheet.Cells["C4"].Value = 150;
            
            worksheet.Cells["A5"].Value = "Furniture";
            worksheet.Cells["B5"].Value = "Table";
            worksheet.Cells["C5"].Value = 250;

            // Skapa en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa aktuellt FieldListSortAscending-värde
            Console.WriteLine("Initial FieldListSortAscending: " + pivotTable.FieldListSortAscending);

            // Visa fältlistan i stigande ordning
            pivotTable.FieldListSortAscending = true;
            Console.WriteLine("FieldListSortAscending set to: " + pivotTable.FieldListSortAscending);

            // Uppdatera och beräkna pivottabellen
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableFieldListSortAscendingDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


