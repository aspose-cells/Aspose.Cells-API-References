---
title: "Class FileFormatInfo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FileFormatInfo-klass. Innehåller data som returneras av FileFormatUtil-metoder för filformatdetektering"
type: docs
url: /sv/net/aspose.cells/fileformatinfo/
---
## FileFormatInfo class

Innehåller data som returneras av [`FileFormatUtil`](../fileformatutil/) metoder för filformatdetektering.

```csharp
public class FileFormatInfo
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [FileFormatInfo](fileformatinfo/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FileFormatType](../../aspose.cells/fileformatinfo/fileformattype/) { get; } | Hämtar det upptäckta filformatet. |
| [IsEncrypted](../../aspose.cells/fileformatinfo/isencrypted/) { get; } | Returnerar true om dokumentet är krypterat och kräver ett lösenord för att öppnas. |
| [IsProtectedByRMS](../../aspose.cells/fileformatinfo/isprotectedbyrms/) { get; } | Indikerar om filen är skyddad av Microsoft Rights Management Server. |
| [LoadFormat](../../aspose.cells/fileformatinfo/loadformat/) { get; } | Hämtar det upptäckta inläsningsformatet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatInfoDemo
    {
        public static void FileFormatInfoExample()
        {
            // Läs in en exempelfil för att upptäcka dess format
            string filePath = "sample.xlsx";
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat(filePath);

            // Visa information om filformat
            Console.WriteLine("File Format Information:");
            Console.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
            Console.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
            Console.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
            Console.WriteLine($"Load Format: {fileInfo.LoadFormat}");

            // Spara informationen till en textfil
            string outputFilePath = "FileFormatInfo.txt";
            using (System.IO.StreamWriter writer = new System.IO.StreamWriter(outputFilePath))
            {
                writer.WriteLine("File Format Information:");
                writer.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
                writer.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
                writer.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
                writer.WriteLine($"Load Format: {fileInfo.LoadFormat}");
            }

            Console.WriteLine($"File format information saved to {outputFilePath}");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


