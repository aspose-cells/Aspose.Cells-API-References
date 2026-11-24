---
title: "LowCodeSplitOptions.LoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSplitOptions-Eigenschaft. Ladeoptionen zum Laden der Tabelle, die aufgeteilt werden soll"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesplitoptions/loadoptions/
---
## LowCodeSplitOptions.LoadOptions property

Ladeoptionen zum Laden der zu teilenden Tabellenkalkulation.

```csharp
public LowCodeLoadOptions LoadOptions { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertyLoadOptionsDemo
    {
        public static void Run()
        {
            // Instanz für Aufteilungsoptionen erstellen
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Ladeoptionen initialisieren
            splitOptions.LoadOptions = new LowCodeLoadOptions();

            // Erstelle neue Ladeoptionen mit unterschiedlichen Einstellungen (unter Verwendung verfügbarer Eigenschaften)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Demonstriere die endgültige Konfiguration
            Console.WriteLine("LoadOptions configured with InputFile: " + splitOptions.LoadOptions.InputFile);
        }
    }
}
```

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


