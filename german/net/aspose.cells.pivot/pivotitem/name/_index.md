---
title: "PivotItem.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotItem-Eigenschaft. Gibt den Namen des Pivot-Elements zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotitem/name/
---
## PivotItem.Name property

Ermittelt den Namen des Pivot-Elements.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyNameDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            ws.Cells["A1"].Value = "Category";
            ws.Cells["B1"].Value = "Value";
            ws.Cells["A2"].Value = "债券借贷";
            ws.Cells["A3"].Value = "股票";
            ws.Cells["A4"].Value = "基金";
            ws.Cells["B2"].Value = 100;
            ws.Cells["B3"].Value = 200;
            ws.Cells["B4"].Value = 300;

            // Pivot-Tabelle erstellen
            int index = ws.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = ws.PivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Greifen Sie auf Pivot-Elemente zu und demonstrieren Sie die Name-Eigenschaft
            PivotField field = pivotTable.RowFields[0];
            foreach (PivotItem item in field.PivotItems)
            {
                // Alle Elemente ausblenden außer "债券借贷"
                item.IsHidden = item.Name != "债券借贷";
                Console.WriteLine($"Pivot Item Name: {item.Name}, Hidden: {item.IsHidden}");
            }
            
            // Aktualisieren und speichern
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            wb.Save("PivotItemNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


