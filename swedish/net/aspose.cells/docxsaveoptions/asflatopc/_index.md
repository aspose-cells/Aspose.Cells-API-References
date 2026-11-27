---
title: "DocxSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocxSaveOptions-egenskap. Anger om sparas som en flat opc-fil som kan genereras av Open XML SDK"
type: docs
url: /sv/net/aspose.cells/docxsaveoptions/asflatopc/
---
## DocxSaveOptions.AsFlatOpc property

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

    public class DocxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Flat OPC Demo";

            try
            {
                // Initiera DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Visa standardvärdet för AsFlatOpc-egenskapen
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Ställ in AsFlatOpc till true för att demonstrera dess användning
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Spara arbetsboken som DOCX med de konfigurerade alternativen
                workbook.Save("AsFlatOpcDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsFlatOpc option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


