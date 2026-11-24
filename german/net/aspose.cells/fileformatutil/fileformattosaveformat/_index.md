---
title: "FileFormatUtil.FileFormatToSaveFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FileFormatUtil Methode. Konvertiert das Dateiformat in das Speicherformat"
type: docs
url: /de/net/aspose.cells/fileformatutil/fileformattosaveformat/
---
## FileFormatUtil.FileFormatToSaveFormat method

Konvertiert das Dateiformat in das Speicherformat.

```csharp
public static SaveFormat FileFormatToSaveFormat(FileFormatType format)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Format | FileFormatType | Der Dateiformattyp. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodFileFormatToSaveFormatWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test FileFormatToSaveFormat");

            // Ermitteln Sie den Dateiformattyp der Arbeitsmappe
            FileFormatType originalFormat = workbook.FileFormat;

            // Konvertieren Sie FileFormatType in SaveFormat
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(originalFormat);

            // Speichern Sie die Arbeitsmappe mit dem konvertierten SaveFormat
            string outputPath = "Output_" + saveFormat.ToString() + ".xlsx";
            workbook.Save(outputPath, saveFormat);

            Console.WriteLine("File saved successfully with SaveFormat: " + saveFormat);
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../saveformat/)
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


