---
title: "DocxSaveOptions.SaveAsEditableShapes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocxSaveOptions-egenskap. Spara alla ritobjekt som redigerbara former i Word-filen så att du kan redigera dem i Word"
type: docs
url: /sv/net/aspose.cells/docxsaveoptions/saveaseditableshapes/
---
## DocxSaveOptions.SaveAsEditableShapes property

Spara alla ritobjekt som redigerbara former i Word‑filen, så att du kan redigera dem i Word.

```csharp
public bool SaveAsEditableShapes { get; set; }
```

### Anmärkningar

Endast för diagram.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertySaveAsEditableShapesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Editable Shapes Demo";

            try
            {
                // Initiera DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Visa standardvärdet för egenskapen SaveAsEditableShapes
                Console.WriteLine("Default SaveAsEditableShapes value: " + saveOptions.SaveAsEditableShapes);

                // Ställ in SaveAsEditableShapes till true för att demonstrera dess användning
                saveOptions.SaveAsEditableShapes = true;
                Console.WriteLine("SaveAsEditableShapes set to: " + saveOptions.SaveAsEditableShapes);

                // Spara arbetsboken som DOCX med de konfigurerade alternativen
                workbook.Save("SaveAsEditableShapesDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with SaveAsEditableShapes option.");
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


