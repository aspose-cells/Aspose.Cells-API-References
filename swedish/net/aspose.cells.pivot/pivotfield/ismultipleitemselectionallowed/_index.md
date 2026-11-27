---
title: "PivotField.IsMultipleItemSelectionAllowed"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Anger om flera objekt kan väljas i sidfältet. Standardvärdet är falskt."
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/
---
## PivotField.IsMultipleItemSelectionAllowed property

Anger om flera objekt kan väljas i sidfältet. Standardvärdet är false.

```csharp
public bool IsMultipleItemSelectionAllowed { get; set; }
```

### Anmärkningar

Endast för sid- (filter)fält.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsMultipleItemSelectionAllowedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            
            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Åtkomst till sidfältet och ange flerval.
            PivotField pageField = pivotTable.PageFields[0];
            pageField.IsMultipleItemSelectionAllowed = true;
            
            // Verifiera att egenskapen har satts
            Console.WriteLine("IsMultipleItemSelectionAllowed: " + pageField.IsMultipleItemSelectionAllowed);
            
            // Spara arbetsboken
            workbook.Save("PivotFieldIsMultipleItemSelectionAllowedDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


