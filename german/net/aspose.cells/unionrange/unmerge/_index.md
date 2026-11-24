---
title: "UnionRange.UnMerge"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Methode. Entfernt die Zusammenführung von zusammengeführten Zellen dieses Bereichs"
type: docs
url: /de/net/aspose.cells/unionrange/unmerge/
---
## UnionRange.UnMerge method

Löst zusammengeführte Zellen dieses Bereichs.

```csharp
public void UnMerge()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Bereich und füge Zellen zusammen
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
            
            // Füge die Zellen zusammen und setze einen Wert
            unionRange.Merge();
            unionRange.PutValue("Merged Cells", true, true);
            
            try
            {
                // Rufe die UnMerge-Methode auf
                unionRange.UnMerge();
                
                Console.WriteLine("Cells unmerged successfully");
                
                // Setze Werte in die nicht zusammengefügten Zellen, um die Wirkung zu demonstrieren
                worksheet.Cells["A1"].PutValue("A1");
                worksheet.Cells["A2"].PutValue("A2");
                worksheet.Cells["B1"].PutValue("B1");
                worksheet.Cells["B2"].PutValue("B2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnMerge method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("MethodUnMergeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


