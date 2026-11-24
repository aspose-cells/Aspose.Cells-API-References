---
title: "Range.EntireColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt ein Range-Objekt zurück, das die gesamte Spalte oder die Spalten darstellt, die den angegebenen Bereich enthalten"
type: docs
url: /de/net/aspose.cells/range/entirecolumn/
---
## Range.EntireColumn property

Liefert ein Range-Objekt, das die gesamte Spalte (oder die gesamten Spalten) enthält, die den angegebenen Bereich umfassen.

```csharp
public Range EntireColumn { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Bereich, beginnend bei Zelle C1 (Zeile 0, Spalte 2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, 1, 1);
            
            // Erhalte die gesamte Spalte, die den Bereich enthält (Spalte C)
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            
            // Formatiere die gesamte Spalte
            Style style = entireColumn[0, 0].GetStyle();
            style.Custom = "##0%";
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            entireColumn.ApplyStyle(style, styleFlag);
            
            // Speichere die Arbeitsmappe
            workbook.Save("EntireColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


