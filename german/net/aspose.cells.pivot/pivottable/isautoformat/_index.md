---
title: "PivotTable.IsAutoFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob der PivotTable-Bericht automatisch formatiert ist. Kontrollkästchen Autoformat-Tabelle, das in den PivotTable-Optionen für Excel 2003 vorhanden ist."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/isautoformat/
---
## PivotTable.IsAutoFormat property

Gibt an, ob der PivotTable-Bericht automatisch formatiert wird. Kontrollkästchen "autoformat table", das in den PivotTable‑Optionen für Excel 2003 vorhanden ist.

```csharp
public bool IsAutoFormat { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsAutoFormatDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);

            // Fügen Sie eine Pivot-Tabelle hinzu
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // PivotTable konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Setze die IsAutoFormat-Eigenschaft
            pivotTable.IsAutoFormat = true; // Enable auto formatting
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableIsAutoFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


