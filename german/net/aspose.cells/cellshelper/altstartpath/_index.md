---
title: "CellsHelper.AltStartPath"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper property. Gibt den alternativen Startpfad zurück oder setzt ihn, der von einigen externen Formelbezügen verwendet wird."
type: docs
url: /de/net/aspose.cells/cellshelper/altstartpath/
---
## CellsHelper.AltStartPath property

Liest oder setzt den alternativen Startpfad, auf den von einigen externen Formelbezügen verwiesen wird.

```csharp
public static string AltStartPath { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyAltStartPathDemo
    {
        public static void Run()
        {
            // Setzen Sie den alternativen Startpfad
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            
            // Setzen Sie außerdem weitere relevante Eigenschaften zur Demonstration
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            
            // Zeigen Sie die Pfade an, um die Verwendung der Eigenschaft zu demonstrieren
            Console.WriteLine("Main Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            
            // Beispiel, wie diese Pfade verwendet werden könnten
            Console.WriteLine("\nWhen resources aren't found in main path, system will check: " + CellsHelper.AltStartPath);
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


