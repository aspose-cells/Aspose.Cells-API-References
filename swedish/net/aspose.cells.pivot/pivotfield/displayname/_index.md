---
title: "PivotField.DisplayName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Representerar visningsnamnet för pivotfältet i pivottabellvyn"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/displayname/
---
## PivotField.DisplayName property

Representerar visningsnamnet för pivotfältet i pivottabellvyn.

```csharp
public string DisplayName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Ange anpassat visningsnamn för datafältet
            pivotTable.DataFields[0].DisplayName = "Total Sales";
            
            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Åtkomst till cell med visningsnamn
            Cell cell = pivotTable.GetCellByDisplayName("Total Sales");
            Console.WriteLine("Cell found at row: {0}, column: {1}", cell.Row, cell.Column);
            
            // Spara arbetsboken
            workbook.Save("PivotFieldDisplayNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


