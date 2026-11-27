---
title: "PivotTable.EnableFieldDialog"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om PivotTable-fältdialogrutan är tillgänglig när användaren dubbelklickar på PivotTable-fältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/enablefielddialog/
---
## PivotTable.EnableFieldDialog property

Anger om dialogrutan för pivottabellfält är tillgänglig när användaren dubbelklickar på pivottabellfältet.

```csharp
public bool EnableFieldDialog { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableFieldDialogDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            var cells = sheet.Cells;
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

            // Demonstrera egenskapen EnableFieldDialog
            pivotTable.EnableFieldDialog = true;
            Console.WriteLine("EnableFieldDialog set to: " + pivotTable.EnableFieldDialog);

            // Ändra egenskapen och verifiera
            pivotTable.EnableFieldDialog = false;
            Console.WriteLine("EnableFieldDialog changed to: " + pivotTable.EnableFieldDialog);

            // Spara arbetsboken
            workbook.Save("PivotTable_EnableFieldDialog_Example.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


