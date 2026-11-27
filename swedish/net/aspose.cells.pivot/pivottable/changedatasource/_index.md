---
title: "PivotTable.ChangeDataSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Ändra datakällan för pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/changedatasource/
---
## PivotTable.ChangeDataSource method

Ändra datakälla för pivottabellen.

```csharp
public void ChangeDataSource(string[] source)
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot; // Added this using directive
    using System;

    public class PivotTableMethodChangeDataSourceWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Skapa en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Förbered ny datakälla
            string[] newDataSource = new string[] { "C1:D4", "Sheet1" };

            try
            {
                // Ändra datakällan för pivottabellen
                pivotTable.ChangeDataSource(newDataSource);

                // Uppdatera pivottabellen för att tillämpa ändringarna
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable data source changed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing pivot table data source: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("PivotTableChangeDataSourceDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


