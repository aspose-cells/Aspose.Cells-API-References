---
title: "PivotField.Items"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Alle Beschriftungen der Pivot-Elemente in diesem Feld abrufen"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/items/
---
## PivotField.Items property

Alle Bezeichnungen der Pivot‑Elemente in diesem Feld abrufen.

```csharp
public string[] Items { get; }
```

### Beispiele

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyItemsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe und füge Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Pivot-Feld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Items-Eigenschaft demonstrieren
            string[] items = pivotField.Items;
            Console.WriteLine("Pivot Field Items:");
            foreach (string item in items)
            {
                Console.WriteLine(item);
            }
            
            // Aktuelles Seiten-Element setzen
            ArrayList list = new ArrayList(items);
            if (list.Contains("Apple"))
            {
                pivotField.CurrentPageItem = (short)list.IndexOf("Apple");
                Console.WriteLine("Current page item set to: Apple");
            }
            
            pivotTable.CalculateData();
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


