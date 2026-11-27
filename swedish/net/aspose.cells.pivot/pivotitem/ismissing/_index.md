---
title: "PivotItem.IsMissing"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem-egenskap. Anger om objektet har tagits bort från datakällan"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/ismissing/
---
## PivotItem.IsMissing property

Anger om objektet har tagits bort från datakällan.

```csharp
public bool IsMissing { get; }
```

### Anmärkningar

Sant betyder att detta värde har tagits bort från datakällan.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsMissingDemo
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
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Uppdatera pivot‑tabellens data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Hämta det första pivot item i det första radfältet
            PivotField rowField = pivotTable.RowFields[0];
            PivotItem pivotItem = rowField.PivotItems[0];

            // Visa värdet för IsMissing-egenskapen
            Console.WriteLine("IsMissing value for '{0}': {1}", pivotItem.Name, pivotItem.IsMissing);

            // Skapa ett scenario där ett objekt kan saknas
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B5"].PutValue(4000);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Kontrollera om det ursprungliga pivot item nu saknas
            Console.WriteLine("After data change - IsMissing value for '{0}': {1}", 
                pivotItem.Name, pivotItem.IsMissing);

            // Spara arbetsboken
            workbook.Save("PivotItemIsMissingDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


