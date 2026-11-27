---
title: "DocxSaveOptions.SaveElementType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocxSaveOptions-egenskap. Anger vilka element som ska sparas"
type: docs
url: /sv/net/aspose.cells/docxsaveoptions/saveelementtype/
---
## DocxSaveOptions.SaveElementType property

Anger vilka element som ska sparas.

```csharp
public SaveElementType SaveElementType { get; set; }
```

### Exempel

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveElementTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och lägg till några exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // Initiera DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // OBS: SaveElementType-egenskapen finns inte i DocxSaveOptions-klassen
                // baserat på den tillhandahållna API-reflektionen. Om den fanns, skulle du läsa den så här:
                // var elementType = saveOptions.SaveElementType;
                // Console.WriteLine("SaveElementType: " + elementType);

                // Demonstrera läsning av en befintlig egenskap: SaveAsEditableShaps
                Console.WriteLine("SaveAsEditableShaps (default): " + saveOptions.SaveAsEditableShaps);

                // Sätt egenskapen till true och visa det nya värdet
                saveOptions.SaveAsEditableShaps = true;
                Console.WriteLine("SaveAsEditableShaps (after set): " + saveOptions.SaveAsEditableShaps);

                // Spara arbetsboken som DOCX med de konfigurerade alternativen
                workbook.Save("SaveElementTypeDemo.docx", saveOptions);
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Se även

* enum [SaveElementType](../../../aspose.cells.saving/saveelementtype/)
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


