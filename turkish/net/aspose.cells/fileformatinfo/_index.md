---
title: "Sınıf FileFormatInfo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "**Aspose.Cells.FileFormatInfo** sınıfı. FileFormatUtil dosya formatı tespit yöntemleri tarafından döndürülen verileri içerir"
type: docs
url: /tr/net/aspose.cells/fileformatinfo/
---
## FileFormatInfo class

[`FileFormatUtil`](../fileformatutil/) tarafından döndürülen verileri içerir, dosya formatı tespit yöntemleri.

```csharp
public class FileFormatInfo
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [FileFormatInfo](fileformatinfo/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FileFormatType](../../aspose.cells/fileformatinfo/fileformattype/) { get; } | Algılanan dosya formatını alır. |
| [IsEncrypted](../../aspose.cells/fileformatinfo/isencrypted/) { get; } | Belge şifrelenmiş ve açmak için bir şifre gerektiriyorsa true döndürür. |
| [IsProtectedByRMS](../../aspose.cells/fileformatinfo/isprotectedbyrms/) { get; } | Dosyanın Microsoft Rights Management Server tarafından korunduğunu gösterir. |
| [LoadFormat](../../aspose.cells/fileformatinfo/loadformat/) { get; } | Algılanan yükleme formatını alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatInfoDemo
    {
        public static void FileFormatInfoExample()
        {
            // Biçimini tespit etmek için bir örnek dosya yükle.
            string filePath = "sample.xlsx";
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat(filePath);

            // Dosya formatı bilgilerini göster.
            Console.WriteLine("File Format Information:");
            Console.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
            Console.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
            Console.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
            Console.WriteLine($"Load Format: {fileInfo.LoadFormat}");

            // Bilgileri bir metin dosyasına kaydet.
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

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


