---
title: "Enum PrintOrderType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PrintOrderType enum. Baskı sırası sabitlerini temsil eder"
type: docs
url: /tr/net/aspose.cells/printordertype/
---
## PrintOrderType enumeration

Yazdırma sırası sabitlerini temsil eder.

```csharp
public enum PrintOrderType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DownThenOver | `0` | Aşağı, ardından sağa |
| OverThenDown | `1` | Sağa, ardından aşağı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintOrderTypeDemo
    {
        public static void PrintOrderTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PageSetup nesnesine erişin
            PageSetup pageSetup = worksheet.PageSetup;

            // Baskı sırasını DownThenOver olarak ayarla
            pageSetup.Order = PrintOrderType.DownThenOver;

            // Demonstrasyon amacıyla bazı diğer sayfa ayarı özelliklerini ayarla
            pageSetup.PrintArea = "A1:D10";
            pageSetup.PrintTitleRows = "$1:$1";
            pageSetup.PrintTitleColumns = "$A:$A";
            pageSetup.CenterHorizontally = true;
            pageSetup.CenterVertically = true;

            // Çalışma kitabını kaydedin
            workbook.Save("PrintOrderTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


