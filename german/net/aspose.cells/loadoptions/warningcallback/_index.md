---
title: "LoadOptions.WarningCallback"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Liest oder setzt den Warn-Callback"
type: docs
url: /de/net/aspose.cells/loadoptions/warningcallback/
---
## LoadOptions.WarningCallback property

Liest oder setzt den Warnungs-Callback.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.Description}");
        }
    }

    public class LoadOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Erstelle einen benutzerdefinierten Warn-Callback
            IWarningCallback warningCallback = new CustomWarningCallback();

            // Initialisiere LoadOptions mit Warn-Callback
            LoadOptions options = new LoadOptions();
            options.WarningCallback = warningCallback;
            options.IgnoreUselessShapes = true;

            // Arbeitsmappe mit Optionen laden
            Workbook workbook = new Workbook("example.xlsx", options);

            // Demonstriere die Verwendung des Warn-Callbacks, indem du eine Zelle zugreifst
            Console.WriteLine($"Cell value: {workbook.Worksheets[0].Cells["A1"].StringValue}");

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


