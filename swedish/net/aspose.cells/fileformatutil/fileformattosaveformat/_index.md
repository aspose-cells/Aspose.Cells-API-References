---
title: "FileFormatUtil.FileFormatToSaveFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatUtil-metoden. Konverterar filformat till sparformat"
type: docs
url: /sv/net/aspose.cells/fileformatutil/fileformattosaveformat/
---
## FileFormatUtil.FileFormatToSaveFormat method

Konverterar filformat till sparaformat.

```csharp
public static SaveFormat FileFormatToSaveFormat(FileFormatType format)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| format | FileFormatType | Filformatstypen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodFileFormatToSaveFormatWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test FileFormatToSaveFormat");

            // Hämta filformatstypen för arbetsboken
            FileFormatType originalFormat = workbook.FileFormat;

            // Konvertera FileFormatType till SaveFormat
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(originalFormat);

            // Spara arbetsboken med det konverterade SaveFormat
            string outputPath = "Output_" + saveFormat.ToString() + ".xlsx";
            workbook.Save(outputPath, saveFormat);

            Console.WriteLine("File saved successfully with SaveFormat: " + saveFormat);
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


