---
title: "LoadOptions.IgnoreUselessShapes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Gibt an, ob nutzlose Formen ignoriert werden"
type: docs
url: /de/net/aspose.cells/loadoptions/ignoreuselessshapes/
---
## LoadOptions.IgnoreUselessShapes property

Gibt an, ob nutzlose Formen ignoriert werden sollen.

```csharp
public bool IgnoreUselessShapes { get; set; }
```

### Hinweise

Funktioniert nur für xlsx-, xlsb- und xlsm-Dateien. Es gibt viele überlappende identische Formen, die in manchen Dateien nutzlos sind; wir können sie beim Laden der Dateien ignorieren.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreUselessShapesDemo
    {
        public static void Run()
        {
            // Ladeoptionen erstellen und IgnoreUselessShapes auf true setzen
            LoadOptions options = new LoadOptions();
            options.IgnoreUselessShapes = true;

            // Lade die Arbeitsmappe mit den Optionen
            Workbook workbook = new Workbook("example.xlsx", options);

            // Gib die Anzahl der Formen im ersten Arbeitsblatt aus
            Console.WriteLine("Shapes count: " + workbook.Worksheets[0].Shapes.Count);
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


