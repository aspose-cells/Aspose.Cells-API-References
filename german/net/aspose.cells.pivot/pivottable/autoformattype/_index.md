---
title: "PivotTable.AutoFormatType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt den automatischen Formattyp der PivotTable zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/autoformattype/
---
## PivotTable.AutoFormatType property

Liest und setzt den automatischen Formattyp der PivotTable.

```csharp
public PivotTableAutoFormatType AutoFormatType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutoFormatTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["C2"].PutValue(1200);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Phone");
            worksheet.Cells["C3"].PutValue(800);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Chair");
            worksheet.Cells["C4"].PutValue(150);
            
            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Felder zu Bereichen hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Category"]);
            pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.BaseFields["Product"]);
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);
            
            // Demonstriere die AutoFormatType-Eigenschaft
            pivotTable.IsAutoFormat = true;
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report6;
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableAutoFormatTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotTableAutoFormatType](../../pivottableautoformattype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


