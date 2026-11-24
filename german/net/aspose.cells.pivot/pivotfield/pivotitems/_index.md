---
title: "PivotField.PivotItems"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField‑Eigenschaft. Gibt die Pivot‑Elemente des PivotFields zurück."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/pivotitems/
---
## PivotField.PivotItems property

Ruft die Pivot‑Elemente des Pivot‑Feldes ab

```csharp
public PivotItemCollection PivotItems { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPivotItemsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["A4"].Value = "A";
            worksheet.Cells["B4"].Value = 30;
            
            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Daten aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Holen Sie das PivotField und demonstrieren Sie PivotItems.
            PivotField field = pivotTable.RowFields[0];
            Console.WriteLine("Field Name: " + field.Name);
            Console.WriteLine("Total PivotItems: " + field.PivotItems.Count);
            
            // Alle Pivot‑Elementnamen anzeigen.
            foreach (PivotItem item in field.PivotItems)
            {
                Console.WriteLine("Item Name: " + item.Name);
            }
        }
    }
}
```

### Siehe auch

* class [PivotItemCollection](../../pivotitemcollection/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


