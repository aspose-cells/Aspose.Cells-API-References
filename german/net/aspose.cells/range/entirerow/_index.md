---
title: "Range.EntireRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt ein Range-Objekt zurück, das die gesamte Zeile oder die Zeilen darstellt, die den angegebenen Bereich enthalten"
type: docs
url: /de/net/aspose.cells/range/entirerow/
---
## Range.EntireRow property

Liefert ein Range-Objekt, das die gesamte Zeile (oder die gesamten Zeilen) enthält, die den angegebenen Bereich umfassen.

```csharp
public Range EntireRow { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füllen Sie einige Beispieldaten in die erste Zeile ein
            for (int col = 0; col < 5; col++)
            {
                sheet.Cells[0, col].PutValue($"Header {col + 1}");
            }

            // Holen Sie die gesamte erste Zeile mit der EntireRow-Eigenschaft
            Aspose.Cells.Range entireRow = sheet.Cells.CreateRange("A1").EntireRow;

            // Kopieren Sie die erste Zeile in die dritte Zeile
            Aspose.Cells.Range destination = sheet.Cells.CreateRange("A3").EntireRow;
            destination.Copy(entireRow);

            // Speichere die Arbeitsmappe
            workbook.Save("EntireRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


