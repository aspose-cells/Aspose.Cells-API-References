---
title: "PivotItem.IsHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotItem-Eigenschaft. Gibt an und legt fest, ob das Pivot-Element ausgeblendet ist"
type: docs
url: /de/net/aspose.cells.pivot/pivotitem/ishidden/
---
## PivotItem.IsHidden property

Liest und setzt, ob das Pivot-Element ausgeblendet ist.

```csharp
public bool IsHidden { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "债券借贷";
            worksheet.Cells["A3"].Value = "股票";
            worksheet.Cells["A4"].Value = "基金";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Zugriff auf Pivot-Feld und -Elemente
            PivotField field = pivotTable.RowFields[0];
            
            // Setze die IsHidden-Eigenschaft, um nur "债券借贷" anzuzeigen
            foreach (PivotItem item in field.PivotItems)
            {
                item.IsHidden = (item.Name != "债券借贷");
            }

            // Pivot-Tabelle aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotItemIsHiddenDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


