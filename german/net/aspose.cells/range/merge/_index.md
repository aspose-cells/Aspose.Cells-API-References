---
title: "Range.Merge"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Kombiniert einen Zellbereich zu einer einzelnen Zelle"
type: docs
url: /de/net/aspose.cells/range/merge/
---
## Range.Merge method

Kombiniert einen Zellenbereich zu einer einzelnen Zelle.

```csharp
public void Merge()
```

### Hinweise

Referenziere die zusammengeführte Zelle über die Adresse der oberen linken Zelle im Bereich.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMergeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Bereich und merge Zellen (3 Zeilen x 2 Spalten)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            range.Merge();

            // Setze den Wert in der zusammengeführten Zelle
            worksheet.Cells[0, 0].Value = "Merged Cells Demo";

            // Formatiere die zusammengeführten Zellen
            Style style = worksheet.Cells[0, 0].GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.IsBold = true;
            worksheet.Cells[0, 0].SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


