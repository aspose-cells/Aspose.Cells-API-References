---
title: "PivotTable.ShowPivotStyleColumnStripes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable‑egenskap. Anger om randformattering tillämpas för kolumnen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/
---
## PivotTable.ShowPivotStyleColumnStripes property

Anger om stripe‑formatering tillämpas för kolumnen.

```csharp
public bool ShowPivotStyleColumnStripes { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleColumnStripesDemo
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
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 12;
            
            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sum of Quantity
            
            // Aktivera kolumnrandning
            pivotTable.ShowPivotStyleColumnStripes = true;
            
            // Spara arbetsboken
            workbook.Save("PivotTableColumnStripesDemo.xlsx");
            
            Console.WriteLine("Pivot table with column stripes created successfully.");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


