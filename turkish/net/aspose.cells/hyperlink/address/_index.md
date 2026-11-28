---
title: "Hyperlink.Address"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Hyperlink özelliği. Bir bağlantının adresini temsil eder"
type: docs
url: /tr/net/aspose.cells/hyperlink/address/
---
## Hyperlink.Address property

Bir köprünün adresini temsil eder.

```csharp
public string Address { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAddressDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Farklı adreslerle bağlantılar ekle
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.baidu.com/");
            worksheet.Hyperlinks.Add("B1", 1, 1, "http://www.google.com/");
            worksheet.Hyperlinks.Add("C1", 1, 1, "Sheet1!F3");

            // Bağlantı adreslerine eriş ve görüntüle
            HyperlinkCollection links = worksheet.Hyperlinks;
            Console.WriteLine("Hyperlink Count: " + links.Count);
            Console.WriteLine("Link 1 Address: " + links[0].Address);
            Console.WriteLine("Link 2 Address: " + links[1].Address);
            Console.WriteLine("Link 3 Address: " + links[2].Address);

            // Çalışma kitabını kaydedin
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


