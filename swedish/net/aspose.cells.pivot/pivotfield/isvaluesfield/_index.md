---
title: "PivotField.IsValuesField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Anger om detta fält representerar värdefältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/isvaluesfield/
---
## PivotField.IsValuesField property

Anger om detta fält representerar värdefält.

```csharp
public bool IsValuesField { get; }
```

### Anmärkningar

Fungerar endast när det finns två eller fler datafält i pivottabellvyn.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyIsValuesFieldDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Sales";

            cells["A2"].Value = "Fruit";
            cells["B2"].Value = "Apple";
            cells["C2"].Value = 100;

            cells["A3"].Value = "Fruit";
            cells["B3"].Value = "Orange";
            cells["C3"].Value = 150;

            cells["A4"].Value = "Vegetable";
            cells["B4"].Value = "Carrot";
            cells["C4"].Value = 200;

            cells["A5"].Value = "Vegetable";
            cells["B5"].Value = "Potato";
            cells["C5"].Value = 250;

            // Lägg till pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // Hämta datafältet (Sales)
                PivotField dataField = pivotTable.DataFields[0];

                // Visa värdet för IsValuesField-egenskapen
                Console.WriteLine("IsValuesField value: " + dataField.IsValuesField);

                // Hämta ett radfält (Category) för jämförelse
                PivotField rowField = pivotTable.RowFields["Category"];
                Console.WriteLine("Row field IsValuesField value: " + rowField.IsValuesField);

                // Beräkna data och uppdatera
                pivotTable.CalculateData();

                // Spara arbetsboken
                workbook.Save("IsValuesFieldDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


