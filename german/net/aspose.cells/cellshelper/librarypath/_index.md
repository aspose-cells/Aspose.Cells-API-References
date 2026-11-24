---
title: "CellsHelper.LibraryPath"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Eigenschaft. Gibt den Bibliothekspfad zurück oder setzt ihn, der von einigen externen Formelbezügen verwendet wird"
type: docs
url: /de/net/aspose.cells/cellshelper/librarypath/
---
## CellsHelper.LibraryPath property

Liest oder setzt den Bibliothekspfad, auf den von einigen externen Formelbezügen verwiesen wird.

```csharp
public static string LibraryPath { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyLibraryPathDemo
    {
        public static void Run()
        {
            // Setze die LibraryPath-Eigenschaft
            CellsHelper.LibraryPath = "C:\\MyLibraries\\AsposeCells";

            // Demonstriere das Abrufen und Verwenden des LibraryPath
            Console.WriteLine("Current Library Path: " + CellsHelper.LibraryPath);

            // Beispiel für die Verwendung des Pfads in einer Dateioperation
            string filePath = System.IO.Path.Combine(CellsHelper.LibraryPath, "test.xlsx");
            Console.WriteLine("Would load file from: " + filePath);
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


