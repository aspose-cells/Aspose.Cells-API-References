---
title: "Enum PrintErrorsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PrintErrorsType enum. Yazdırma hataları sabitlerini temsil eder"
type: docs
url: /tr/net/aspose.cells/printerrorstype/
---
## PrintErrorsType enumeration

Yazdırma hataları sabitlerini temsil eder.

```csharp
public enum PrintErrorsType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| PrintErrorsBlank | `0` | Hataların yazdırılmamasını temsil eder. |
| PrintErrorsDash | `1` | Hataları "--" olarak yazdırmayı temsil eder. |
| PrintErrorsDisplayed | `2` | Hataları görüntülendiği gibi yazdırmayı temsil eder. |
| PrintErrorsNA | `3` | Hataları "#N/A" olarak yazdırmayı temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintErrorsTypeDemo
    {
        public static void PrintErrorsTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasının PageSetup'ına eriş
            PageSetup pageSetup = worksheet.PageSetup;

            // Farklı yazdırma hata türlerini ayarla
            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            workbook.Save("PrintErrorsBlank.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            workbook.Save("PrintErrorsDash.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
            workbook.Save("PrintErrorsDisplayed.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsNA;
            workbook.Save("PrintErrorsNA.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


