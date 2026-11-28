---
title: "XmlLoadOptions.DateFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlLoadOptions özelliği. Tarih değerinin biçimini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/xmlloadoptions/dateformat/
---
## XmlLoadOptions.DateFormat property

Tarih değerinin biçimini alır ve ayarlar.

```csharp
public string DateFormat { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // XmlLoadOptions sınıfının bir örneğini oluştur.
            XmlLoadOptions options = new XmlLoadOptions();

            // XML'den tarihleri ayrıştırmak için tarih biçimini ayarlayın
            options.DateFormat = "yyyy-MM-dd";
            options.ConvertNumericOrDate = true;

            // Belirtilen seçenekleri kullanarak bir XML dosyasını Çalışma Kitabı'na yükle.
            Workbook workbook = new Workbook("input.xml", options);

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Tarih biçimlendirmesini göstermek için bazı hücreleri görüntüleyin
            Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].Value);

            // Çalışma kitabını yeni bir dosyaya kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


