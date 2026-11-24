---
title: "PptxSaveOptions.PptxSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PptxSaveOptions-Konstruktor. Stellt die PPTX-Speicheroptionen dar."
type: docs
url: /de/net/aspose.cells/pptxsaveoptions/pptxsaveoptions/
---
## PptxSaveOptions() {#constructor}

Stellt die pptx-Speicheroptionen dar.

```csharp
public PptxSaveOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Visible Data");
            worksheet.Cells["A2"].PutValue("Hidden Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // Verstecke die zweite Zeile
            worksheet.Cells.Rows[1].IsHidden = true;

            // PptxSaveOptions mit dem Konstruktor erstellen
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;

            // Arbeitsmappe mit Optionen als PPTX speichern
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved to PPTX with hidden rows ignored.");
        }
    }
}
```

### Siehe auch

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PptxSaveOptions(bool) {#constructor_1}

Repräsentiert Optionen zum Speichern einer .pptx‑Datei.

```csharp
public PptxSaveOptions(bool saveAsImage)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveAsImage | Boolean | Wenn True, wird die Arbeitsmappe in einige Bilder der .pptx-Datei konvertiert. Wenn False, wird die Arbeitsmappe in einige Tabellen der .pptx-Datei konvertiert. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            try
            {
                // Rufen Sie die #ctor-Methode mit einem booleschen Parameter auf
                bool saveAsImage = true;
                PptxSaveOptions options = new PptxSaveOptions(saveAsImage);

                // Zusätzliche Eigenschaften festlegen
                options.IgnoreHiddenRows = true;
                options.ExportViewType = SlideViewType.View;

                // Die Arbeitsmappe mit PPTX-Optionen speichern
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

### Siehe auch

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


