---
title: "PivotTable.EnableWizard"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om PivotTable‑guiden är tillgänglig"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/enablewizard/
---
## PivotTable.EnableWizard property

Anger om pivottabellguiden är tillgänglig.

```csharp
public bool EnableWizard { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableWizardDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 2000;

            // Lägg till pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Inaktivera pivottabellsguiden
            pivotTable.EnableWizard = false;

            // Spara arbetsboken
            workbook.Save("PivotTable_EnableWizard_Demo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


