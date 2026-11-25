---
title: "FileFormatInfo.FileFormatType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FileFormatInfo. Ottiene il formato file rilevato"
type: docs
url: /it/net/aspose.cells/fileformatinfo/fileformattype/
---
## FileFormatInfo.FileFormatType property

Ottiene il formato file rilevato.

```csharp
public FileFormatType FileFormatType { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // Esempio 1: Rileva il formato Excel 97-2003
            string excelFile = "sample.xls";
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(excelFile);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            Console.WriteLine("Is Encrypted: " + info.IsEncrypted);

            // Esempio 2: Rileva il formato OOXML
            string xlsxFile = "sample.xlsx";
            info = FileFormatUtil.DetectFileFormat(xlsxFile);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            Console.WriteLine("Is Encrypted: " + info.IsEncrypted);
        }
    }
}
```

### Vedi anche

* enum [FileFormatType](../../fileformattype/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


