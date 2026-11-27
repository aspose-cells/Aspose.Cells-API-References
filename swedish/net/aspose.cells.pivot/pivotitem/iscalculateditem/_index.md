---
title: "PivotItem.IsCalculatedItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem-egenskap. Anger om detta pivotelement är ett beräknat formel‑element"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/iscalculateditem/
---
## PivotItem.IsCalculatedItem property

Anger om detta pivotelement är ett beräknat formelobjekt.

```csharp
public bool IsCalculatedItem { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsCalculatedItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 15;

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Beräkna pivottabellsdata
            pivotTable.CalculateData();

            // Hämta det första pivotelementet från det första pivotfältet
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // Visa värdet för egenskapen IsCalculatedItem
            Console.WriteLine("IsCalculatedItem value: " + pivotItem.IsCalculatedItem);

            // Kontrollera om pivotelementet är ett beräknat element
            if (pivotItem.IsCalculatedItem)
            {
                Console.WriteLine("This pivot item is a calculated formula item.");
                Console.WriteLine("Formula: " + pivotItem.GetFormula());
            }
            else
            {
                Console.WriteLine("This pivot item is not a calculated formula item.");
            }

            // Spara arbetsboken
            workbook.Save("PivotItemPropertyIsCalculatedItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


