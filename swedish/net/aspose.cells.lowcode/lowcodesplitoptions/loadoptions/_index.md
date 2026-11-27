---
title: "LowCodeSplitOptions.LoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSplitOptions‑egenskap. Laddningsalternativ för att läsa in kalkylbladet som ska delas"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesplitoptions/loadoptions/
---
## LowCodeSplitOptions.LoadOptions property

Läsalternativ för att läsa in kalkylbladet som ska delas upp.

```csharp
public LowCodeLoadOptions LoadOptions { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertyLoadOptionsDemo
    {
        public static void Run()
        {
            // Skapa en instans av delningsalternativ
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Initiera laddningsalternativ
            splitOptions.LoadOptions = new LowCodeLoadOptions();

            // Skapa nya laddningsalternativ med olika inställningar (med hjälp av tillgängliga egenskaper)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Visa slutlig konfiguration
            Console.WriteLine("LoadOptions configured with InputFile: " + splitOptions.LoadOptions.InputFile);
        }
    }
}
```

### Se även

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


