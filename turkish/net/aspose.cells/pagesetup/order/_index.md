---
title: "PageSetup.Order"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Microsoft Excel'in büyük bir çalışma sayfasını yazdırırken sayfaları numaralandırmak için kullandığı sıralamayı temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/order/
---
## PageSetup.Order property

Microsoft Excel'in büyük bir çalışma sayfasını yazdırırken sayfaları numaralandırmak için kullandığı sıralamayı temsil eder.

```csharp
public PrintOrderType Order { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrderDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Baskı sırasını DownThenOver olarak ayarla
            sheet.PageSetup.Order = PrintOrderType.DownThenOver;
            Console.WriteLine("Print order set to: " + sheet.PageSetup.Order);

            // Çalışma kitabını farklı formatlarda kaydedin
            workbook.Save("output_DownThenOver.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_DownThenOver.xls", SaveFormat.Excel97To2003);

            // Yazdırma sırasını OverThenDown olarak değiştir
            sheet.PageSetup.Order = PrintOrderType.OverThenDown;
            Console.WriteLine("Print order changed to: " + sheet.PageSetup.Order);

            // Farklı formatlarla tekrar kaydet
            workbook.Save("output_OverThenDown.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_OverThenDown.xls", SaveFormat.Excel97To2003);
        }
    }
}
```

### Ayrıca Bakınız

* enum [PrintOrderType](../../printordertype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


