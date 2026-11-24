---
title: "PivotTable.BaseFields"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt alle Basis-Pivot-Felder in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/basefields/
---
## PivotTable.BaseFields property

Gibt alle Basis-Pivot-Felder in der PivotTable zurück.

```csharp
public PivotFieldCollection BaseFields { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyBaseFieldsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
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
            int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Pivot-Tabellendaten aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Greife auf die BaseFields-Sammlung zu
            PivotFieldCollection baseFields = pivotTable.BaseFields;
            
            // Zeige originale Elemente jedes Basisfelds an
            Console.WriteLine("Base Fields and their Original Items:");
            foreach (PivotField field in baseFields)
            {
                Console.WriteLine($"Field: {field.Name}");
                string[] originalItems = field.OriginalItems;
                foreach (string item in originalItems)
                {
                    Console.WriteLine($"- {item}");
                }
            }
        }
    }
}
```

### Siehe auch

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


