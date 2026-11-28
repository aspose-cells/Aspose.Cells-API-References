---
title: "FileFormatUtil.FileFormatToSaveFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FileFormatUtil yöntemi. Dosya biçimini kaydetme biçimine dönüştürme"
type: docs
url: /tr/net/aspose.cells/fileformatutil/fileformattosaveformat/
---
## FileFormatUtil.FileFormatToSaveFormat method

Dosya formatını kaydetme formatına dönüştürme.

```csharp
public static SaveFormat FileFormatToSaveFormat(FileFormatType format)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| biçim | FileFormatType | Dosya biçimi türü. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodFileFormatToSaveFormatWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test FileFormatToSaveFormat");

            // Çalışma kitabının dosya biçimi türünü al
            FileFormatType originalFormat = workbook.FileFormat;

            // FileFormatType'ı SaveFormat'a dönüştür
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(originalFormat);

            // Dönüştürülmüş SaveFormat'ı kullanarak çalışma kitabını kaydet
            string outputPath = "Output_" + saveFormat.ToString() + ".xlsx";
            workbook.Save(outputPath, saveFormat);

            Console.WriteLine("File saved successfully with SaveFormat: " + saveFormat);
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveFormat](../../saveformat/)
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


