---
title: "FileFormatInfo.LoadFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FileFormatInfo özelliği. Algılanan yükleme biçimini alır"
type: docs
url: /tr/net/aspose.cells/fileformatinfo/loadformat/
---
## FileFormatInfo.LoadFormat property

Algılanan yükleme formatını alır.

```csharp
public LoadFormat LoadFormat { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Belgeler dizinine giden yol.
            string filePath = "data/";
            
            // Dosya formatını algıla
            string fileName = "SAMPLE_XLS_ISSUE.XLS";
            var fileFormatInfo = FileFormatUtil.DetectFileFormat(filePath + fileName);
            Console.WriteLine("Detected LoadFormat: " + fileFormatInfo.LoadFormat);

            // Dosyayı doğru biçimde yükle
            LoadOptions loadOptions = new LoadOptions(LoadFormat.MHtml);
            var workbook = new Workbook(filePath + fileName, loadOptions);
            
            // Çalışma kitabını işle
            workbook.Worksheets[0].AutoFitColumns();
            workbook.Save(filePath + "output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [LoadFormat](../../loadformat/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


