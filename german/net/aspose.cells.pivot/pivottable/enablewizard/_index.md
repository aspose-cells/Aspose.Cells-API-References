---
title: "PivotTable.EnableWizard"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob der PivotTable-Assistent verfügbar ist"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/enablewizard/
---
## PivotTable.EnableWizard property

Gibt an, ob der PivotTable‑Assistent verfügbar ist.

```csharp
public bool EnableWizard { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 2000;

            // PivotTable hinzufügen
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // PivotTable-Assistent deaktivieren
            pivotTable.EnableWizard = false;

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTable_EnableWizard_Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


