---
title: "PptxSaveOptions.PptxSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PptxSaveOptions-konstruktor. Representerar PPTX-sparalternativen"
type: docs
url: /sv/net/aspose.cells/pptxsaveoptions/pptxsaveoptions/
---
## PptxSaveOptions() {#constructor}

Representerar pptx‑sparaalternativen.

```csharp
public PptxSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Visible Data");
            worksheet.Cells["A2"].PutValue("Hidden Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // Dölj den andra raden
            worksheet.Cells.Rows[1].IsHidden = true;

            // Skapa PptxSaveOptions med hjälp av konstruktorn
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;

            // Spara arbetsboken till PPTX med alternativ
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved to PPTX with hidden rows ignored.");
        }
    }
}
```

### Se även

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PptxSaveOptions(bool) {#constructor_1}

Representerar alternativ för att spara .pptx‑filen.

```csharp
public PptxSaveOptions(bool saveAsImage)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveAsImage | Boolean | Om True konverteras arbetsboken till några bilder i .pptx-filen. Om False konverteras arbetsboken till några tabeller i .pptx-filen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slides;
    using System;

    public class PptxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            try
            {
                // Anropa #ctor-metoden med boolesk parameter
                bool saveAsImage = true;
                PptxSaveOptions options = new PptxSaveOptions(saveAsImage);

                // Ange ytterligare egenskaper
                options.IgnoreHiddenRows = true;
                options.ExportViewType = SlideViewType.View;

                // Spara arbetsboken med PPTX-alternativ
                workbook.Save("PptxSaveOptionsCtorDemo.pptx", options);

                Console.WriteLine("PptxSaveOptions constructor executed successfully with parameter: " + saveAsImage);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PptxSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


