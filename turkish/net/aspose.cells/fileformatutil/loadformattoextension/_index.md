---
title: "FileFormatUtil.LoadFormatToExtension"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FileFormatUtil yöntemi. Bir yükleme biçimi enum değerini dosya uzantısına dönüştürür."
type: docs
url: /tr/net/aspose.cells/fileformatutil/loadformattoextension/
---
## FileFormatUtil.LoadFormatToExtension method

Yükleme formatı enum değerini dosya uzantısına dönüştürür.

```csharp
public static string LoadFormatToExtension(LoadFormat loadFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadFormat | LoadFormat | Yüklenen dosya biçimi. |

### Dönüş Değeri

Döndürülen uzantı, başında nokta olan küçük harfli bir dizedir.

### Açıklamalar

Dönüştürülemezse, null döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodLoadFormatToExtensionWithLoadFormatDemo
    {
        public static void Run()
        {
            // LoadFormatToExtension'i çeşitli LoadFormat değerleriyle gösterin
            Console.WriteLine("Auto format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Auto));
            Console.WriteLine("CSV format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Csv));
            Console.WriteLine("Excel97-2003 format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Excel97To2003));
            Console.WriteLine("XLSX format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsx));
            Console.WriteLine("TSV format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Tsv));
            Console.WriteLine("ODS format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Ods));
            Console.WriteLine("XLSB format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsb));
        }
    }
}
```

### Ayrıca Bakınız

* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


