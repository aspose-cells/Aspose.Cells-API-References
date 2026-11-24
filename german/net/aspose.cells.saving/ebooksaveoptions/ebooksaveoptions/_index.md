---
title: "EbookSaveOptions.EbookSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EbookSaveOptions‑Konstruktor. Erstellt Optionen zum Speichern einer Ebook‑Datei"
type: docs
url: /de/net/aspose.cells.saving/ebooksaveoptions/ebooksaveoptions/
---
## EbookSaveOptions() {#constructor}

Erstellt Optionen zum Speichern von E‑Book‑Dateien.

```csharp
public EbookSaveOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class EbookSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispielinhalt hinzufügen
            worksheet.Cells["A1"].PutValue("Ebook Test");
            worksheet.Cells["A2"].PutValue("This is a test for EbookSaveOptions");
            
            // Erstelle EbookSaveOptions mit dem Konstruktor
            EbookSaveOptions saveOptions = new EbookSaveOptions();
            
            // Speichere die Arbeitsmappe mit EbookSaveOptions (speichert automatisch als EPUB)
            workbook.Save("output.epub", saveOptions);
            
            Console.WriteLine("Ebook saved successfully with EbookSaveOptions constructor.");
        }
    }
}
```

### Siehe auch

* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)

---

## EbookSaveOptions(SaveFormat) {#constructor_1}

Erstellt Optionen zum Speichern von E‑Book‑Dateien.

```csharp
public EbookSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveFormat | SaveFormat | Das Dateiformat. Es sollte Epub oder Azw3 sein. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Sample Ebook Content");
            
            try
            {
                // Rufen Sie die #ctor-Methode mit dem SaveFormat-Parameter auf
                EbookSaveOptions saveOptions = new EbookSaveOptions(SaveFormat.Epub);
                
                // Setzen Sie bei Bedarf zusätzliche Eigenschaften
                saveOptions.Encoding = System.Text.Encoding.UTF8;
                
                Console.WriteLine("EbookSaveOptions constructor executed successfully with SaveFormat.Epub");
                
                // Speichern Sie die Arbeitsmappe mit den erstellten Optionen
                workbook.Save("EbookSaveOptionsDemo.epub", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


