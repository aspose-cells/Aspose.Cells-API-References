---
title: "PivotArea.AxisType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotArea property. Liest und setzt den Bereich der PivotTable, auf den diese Regel angewendet wird"
type: docs
url: /de/net/aspose.cells.pivot/pivotarea/axistype/
---
## PivotArea.AxisType property

Liest und setzt den Bereich der PivotTable, für den diese Regel gilt.

```csharp
public PivotFieldType AxisType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyAxisTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 800;

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Fügt Felder zu Pivot-Bereichen hinzu.
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Sales

            // PivotArea erstellen und konfigurieren
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row; // Demonstrate AxisType property
            pivotArea.RuleType = PivotAreaType.Normal;

            // Pivotbereich auswählen
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotAreaAxisTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


