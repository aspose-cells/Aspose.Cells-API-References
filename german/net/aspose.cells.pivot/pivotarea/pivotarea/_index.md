---
title: "PivotArea.PivotArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotArea-Konstruktor. Gibt den ausgewählten Bereich der PivotTable wieder"
type: docs
url: /de/net/aspose.cells.pivot/pivotarea/pivotarea/
---
## PivotArea constructor

Stellt den ausgewählten Bereich der PivotTable dar.

```csharp
public PivotArea(PivotTable table)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Tabelle | PivotTable |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodctorWithPivotTableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Demonstriere den PivotArea-Konstruktor mit dem PivotTable-Parameter
            PivotArea pivotArea = new PivotArea(pivotTable);
            
            // Pivot-Bereich konfigurieren
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotAreaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


