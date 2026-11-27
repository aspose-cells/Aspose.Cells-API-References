---
title: "FileFormatInfo.LoadFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatInfo-egenskap. Hämtar det upptäckta inläsningsformatet"
type: docs
url: /sv/net/aspose.cells/fileformatinfo/loadformat/
---
## FileFormatInfo.LoadFormat property

Hämtar det upptäckta inläsningsformatet.

```csharp
public LoadFormat LoadFormat { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Sökvägen till dokumentkatalogen.
            string filePath = "data/";
            
            // Detektera filformat
            string fileName = "SAMPLE_XLS_ISSUE.XLS";
            var fileFormatInfo = FileFormatUtil.DetectFileFormat(filePath + fileName);
            Console.WriteLine("Detected LoadFormat: " + fileFormatInfo.LoadFormat);

            // Läs in fil med korrekt format
            LoadOptions loadOptions = new LoadOptions(LoadFormat.MHtml);
            var workbook = new Workbook(filePath + fileName, loadOptions);
            
            // Bearbeta arbetsboken
            workbook.Worksheets[0].AutoFitColumns();
            workbook.Save(filePath + "output.xlsx");
        }
    }
}
```

### Se även

* enum [LoadFormat](../../loadformat/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


