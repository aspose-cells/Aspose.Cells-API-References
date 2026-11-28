---
title: "Sınıf FileFormatUtil"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FileFormatUtil sınıfı. Dosya formatı enumlarını dize veya dosya uzantılarına ve geri dönüştürmek için yardımcı yöntemler sağlar"
type: docs
url: /tr/net/aspose.cells/fileformatutil/
---
## FileFormatUtil class

Dosya formatı enumlarını stringlere veya dosya uzantılarına ve geri dönüştürmek için yardımcı yöntemler sağlar.

```csharp
public class FileFormatUtil
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat)(Stream) | Bir akışta depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_2)(string) | Bir dosyada depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_1)(Stream, string) | Bir akışta depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_3)(string, string) | Bir dosyada depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür. |
| static [ExtensionToSaveFormat](../../aspose.cells/fileformatutil/extensiontosaveformat/)(string) | Bir dosya adı uzantısını SaveFormat değerine dönüştürür. |
| static [FileFormatToSaveFormat](../../aspose.cells/fileformatutil/fileformattosaveformat/)(FileFormatType) | Dosya formatını kaydetme formatına dönüştürme. |
| static [IsTemplateFormat](../../aspose.cells/fileformatutil/istemplateformat/)(string) | Uzantı .xlt, .xltX, .xltm, .ots ise true döndürür. |
| static [LoadFormatToExtension](../../aspose.cells/fileformatutil/loadformattoextension/)(LoadFormat) | Yükleme formatı enum değerini dosya uzantısına dönüştürür. |
| static [LoadFormatToSaveFormat](../../aspose.cells/fileformatutil/loadformattosaveformat/)(LoadFormat) | Mümkünse LoadFormat değerini SaveFormat değerine dönüştürür. |
| static [SaveFormatToExtension](../../aspose.cells/fileformatutil/saveformattoextension/)(SaveFormat) | Kaydetme formatı enum değerini dosya uzantısına dönüştürür. |
| static [SaveFormatToLoadFormat](../../aspose.cells/fileformatutil/saveformattoloadformat/)(SaveFormat) | Mümkünse SaveFormat değerini LoadFormat değerine dönüştürür. |
| static [VerifyPassword](../../aspose.cells/fileformatutil/verifypassword/)(Stream, string) | Bir akışta depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFileFormatUtilDemo
    {
        public static void Run()
        {
            string filePath = "example.xlt";
            
            // Dosya formatını algıla
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            Console.WriteLine("Detected file format: " + info.FileFormatType);
            
            // Workbook ile dosya formatını doğrula
            Workbook workbook = new Workbook(filePath);
            Console.WriteLine("Workbook file format: " + workbook.FileFormat);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


