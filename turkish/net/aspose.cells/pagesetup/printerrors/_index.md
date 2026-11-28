---
title: "PageSetup.PrintErrors"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Görüntülenen yazdırma hatası türünü belirtir."
type: docs
url: /tr/net/aspose.cells/pagesetup/printerrors/
---
## PageSetup.PrintErrors property

Görüntülenen yazdırma hatası türünü belirtir.

```csharp
public PrintErrorsType PrintErrors { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintErrorsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Yazdırma hatalarını boş olarak görüntülenecek şekilde ayarla
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            Console.WriteLine("PrintErrors set to: " + sheet.PageSetup.PrintErrors);
            
            // Yazdırma hatalarını tire olarak görüntülenecek şekilde değiştir
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            Console.WriteLine("PrintErrors changed to: " + sheet.PageSetup.PrintErrors);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PrintErrorsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PrintErrorsType](../../printerrorstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


