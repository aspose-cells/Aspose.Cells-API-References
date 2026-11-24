---
title: "CellsHelper.StartupPath"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Eigenschaft. Gibt den Startpfad zurück oder legt ihn fest, auf den sich einige externe Formelbezüge beziehen"
type: docs
url: /de/net/aspose.cells/cellshelper/startuppath/
---
## CellsHelper.StartupPath property

Liest oder setzt den Startpfad, auf den von einigen externen Formelbezügen verwiesen wird.

```csharp
public static string StartupPath { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyStartupPathDemo
    {
        public static void Run()
        {
            // Setzen Sie den Startpfad
            CellsHelper.StartupPath = "C:\\Temp\\AsposeCellsStartup";
            
            // Startpfad anzeigen
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);

            // Zusätzliche CellsHelper-Eigenschaften demonstrieren
            CellsHelper.SignificantDigits = 15;
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


