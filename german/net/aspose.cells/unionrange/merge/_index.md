---
title: "UnionRange.Merge"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Methode. Kombiniert einen Zellbereich zu einer einzelnen Zelle"
type: docs
url: /de/net/aspose.cells/unionrange/merge/
---
## UnionRange.Merge method

Kombiniert einen Zellenbereich zu einer einzelnen Zelle.

```csharp
public void Merge()
```

### Hinweise

Referenziere die zusammengeführte Zelle über die Adresse der oberen linken Zelle im Bereich.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodMergeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Zellbereich (A1:B2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            
            // Füge einige Daten in die Zellen ein, um das Zusammenführen zu visualisieren
            range[0, 0].PutValue("Before Merge");
            range[0, 1].PutValue("A1");
            range[1, 0].PutValue("B1");
            range[1, 1].PutValue("B2");
            
            try
            {
                // Erstelle ein UnionRange aus dem Bereich
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
                
                // Rufe die Merge-Methode auf
                unionRange.Merge();
                
                // Setze einen Wert in die zusammengeführte Zelle
                unionRange.PutValue("Merged A1:B2", true, true);
                
                Console.WriteLine("Cells merged successfully");
                
                // Entkommentiere, um die Wirkung des Aufteilens zu sehen
                // unionRange.UnMerge();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Merge method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("MethodMergeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


