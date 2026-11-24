---
title: "PasteOptions.Transpose"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PasteOptions-Eigenschaft. Wahr, um Zeilen und Spalten beim Einfügen des Bereichs zu transponieren. Der Standardwert ist Falsch"
type: docs
url: /de/net/aspose.cells/pasteoptions/transpose/
---
## PasteOptions.Transpose property

True, um Zeilen und Spalten beim Einfügen des Bereichs zu transponieren. Der Standardwert ist False.

```csharp
public bool Transpose { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyTransposeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Quellstil erstellen und auf den horizontalen Bereich anwenden
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range sourceRange = cells.CreateRange(0, 0, 1, 4);
            sourceRange.SetStyle(style);

            // Paste-Optionen mit Transponierung erstellen
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.Formats;
            pasteOptions.Transpose = true;

            // Kopieren mit Transponierung in einen vertikalen Bereich
            Aspose.Cells.Range targetRange = cells.CreateRange(2, 0, 4, 1);
            targetRange.Copy(sourceRange, pasteOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("TransposeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


