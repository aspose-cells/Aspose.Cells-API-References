---
title: "Range.IsBlank"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Gibt an, ob der Bereich Werte enthält"
type: docs
url: /de/net/aspose.cells/range/isblank/
---
## Range.IsBlank method

Gibt an, ob der Bereich Werte enthält.

```csharp
public bool IsBlank()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstelle einen Bereich und prüfe, ob er leer ist (sollte wahr sein)
            Aspose.Cells.Range range1 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank: " + range1.IsBlank());

            // Setze einen Wert in eine Zelle und prüfe erneut (sollte falsch sein)
            cells["B2"].PutValue("Test");
            Aspose.Cells.Range range2 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank after adding value: " + range2.IsBlank());
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


