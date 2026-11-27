---
title: "DocxSaveOptions.AsNormalView"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocxSaveOptions‑egenskap. Exporterar Excel‑fil till docx‑fil som normal vy. Om denna egenskap är true kommer ett område att exporteras och ingen skala kommer att tillämpas. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/docxsaveoptions/asnormalview/
---
## DocxSaveOptions.AsNormalView property

Exporterar Excel‑fil till docx‑fil som normal vy. Om den här egenskapen är sann kommer ett område att exporteras, och ingen skala kommer att tillämpas. Standardvärdet är falskt.

```csharp
public bool AsNormalView { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsNormalViewDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Normal View Demo";

            try
            {
                // Initiera DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Visa standardvärdet för egenskapen AsNormalView
                Console.WriteLine("Default AsNormalView value: " + saveOptions.AsNormalView);

                // Ställ in AsNormalView till true för att demonstrera dess användning
                saveOptions.AsNormalView = true;
                Console.WriteLine("AsNormalView set to: " + saveOptions.AsNormalView);

                // Spara arbetsboken som DOCX med de konfigurerade alternativen
                workbook.Save("AsNormalViewDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsNormalView option.");
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


