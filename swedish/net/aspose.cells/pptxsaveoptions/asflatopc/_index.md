---
title: "PptxSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PptxSaveOptions‑egenskap. Anger om sparandet sker som en flat opc‑fil som kan genereras av Open XML SDK"
type: docs
url: /sv/net/aspose.cells/pptxsaveoptions/asflatopc/
---
## PptxSaveOptions.AsFlatOpc property

Anger om sparning som en platt opc‑fil som kan genereras av Open XML SDK

```csharp
public bool AsFlatOpc { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PptxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Flat OPC Demo";

            try
            {
                // Skapa en PptxSaveOptions‑instans
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // Visa standardvärdet för AsFlatOpc
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Ställ in egenskapen till true för att demonstrera dess användning
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Spara arbetsboken som PPTX med alternativet aktiverat
                workbook.Save("AsFlatOpcDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with AsFlatOpc enabled");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


