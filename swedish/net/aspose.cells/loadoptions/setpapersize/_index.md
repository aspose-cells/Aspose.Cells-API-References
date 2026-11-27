---
title: "LoadOptions.SetPaperSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions‑metod. Ställer in standardpappersstorlek för utskrift baserat på standardskrivarens inställning"
type: docs
url: /sv/net/aspose.cells/loadoptions/setpapersize/
---
## LoadOptions.SetPaperSize method

Anger standardpappersstorlek för utskrift från standardskrivarens inställning.

```csharp
public void SetPaperSize(PaperSizeType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | PaperSizeType | Standardpappersstorleken. |

### Anmärkningar

Om det inte finns någon inställning för pappersstorlek, kommer MS Excel att använda standardinställningen för skrivaren.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsMethodSetPaperSizeWithPaperSizeTypeDemo
    {
        public static void Run()
        {
            // Skapa inläsningsalternativ och ställ in pappersstorlek till A5
            LoadOptions options = new LoadOptions();
            options.SetPaperSize(PaperSizeType.PaperA5);

            // Läs in arbetsbok med de angivna alternativen
            Workbook workbook = new Workbook("example.xlsx", options);
            
            // Verifiera att papperstorleken är korrekt inställd
            Console.WriteLine("Paper size of first worksheet: " + workbook.Worksheets[0].PageSetup.PaperSize);
        }
    }
}
```

### Se även

* enum [PaperSizeType](../../papersizetype/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


