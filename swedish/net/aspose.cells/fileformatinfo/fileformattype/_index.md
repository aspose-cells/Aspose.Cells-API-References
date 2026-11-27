---
title: "FileFormatInfo.FileFormatType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatInfo-egenskap. Hämtar det upptäckta filformatet"
type: docs
url: /sv/net/aspose.cells/fileformatinfo/fileformattype/
---
## FileFormatInfo.FileFormatType property

Hämtar det upptäckta filformatet.

```csharp
public FileFormatType FileFormatType { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // Exempel 1: Detektera Excel 97-2003-format
            string excelFile = "sample.xls";
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(excelFile);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            Console.WriteLine("Is Encrypted: " + info.IsEncrypted);

            // Exempel 2: Detektera OOXML-format
            string xlsxFile = "sample.xlsx";
            info = FileFormatUtil.DetectFileFormat(xlsxFile);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            Console.WriteLine("Is Encrypted: " + info.IsEncrypted);
        }
    }
}
```

### Se även

* enum [FileFormatType](../../fileformattype/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


