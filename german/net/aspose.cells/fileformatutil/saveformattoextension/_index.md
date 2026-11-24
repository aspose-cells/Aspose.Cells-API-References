---
title: "FileFormatUtil.SaveFormatToExtension"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FileFormatUtil-Methode. Konvertiert einen enumerierten SaveFormat-Wert in eine Dateierweiterung"
type: docs
url: /de/net/aspose.cells/fileformatutil/saveformattoextension/
---
## FileFormatUtil.SaveFormatToExtension method

Konvertiert einen SaveFormat-Enum-Wert in eine Dateierweiterung.

```csharp
public static string SaveFormatToExtension(SaveFormat format)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Format | SaveFormat | Das Speicherformat. |

### Rückgabewert

Die zurückgegebene Erweiterung ist ein Kleinbuchstaben-String mit einem führenden Punkt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToExtensionWithSaveFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test content");

            // Demonstriere SaveFormatToExtension mit verschiedenen Formaten
            SaveOptions[] saveOptions = {
                new PdfSaveOptions(),
                new XlsSaveOptions(SaveFormat.Excel97To2003),
                new OoxmlSaveOptions(SaveFormat.Xlsx),
                new OdsSaveOptions()
            };

            foreach (var options in saveOptions)
            {
                string extension = FileFormatUtil.SaveFormatToExtension(options.SaveFormat);
                Console.WriteLine($"SaveFormat: {options.SaveFormat} -> Extension: {extension}");
                
                // Speichere mit der erkannten Erweiterung
                string fileName = $"output{extension}";
                workbook.Save(fileName, options);
                Console.WriteLine($"Saved file: {fileName}");
            }

            workbook.Dispose();
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


