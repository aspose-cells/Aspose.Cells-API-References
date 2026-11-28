---
title: "Sınıf XmlDataBinding"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.XmlDataBinding sınıfı. Xml Veri Bağlama bilgilerini temsil eder."
type: docs
url: /tr/net/aspose.cells/xmldatabinding/
---
## XmlDataBinding class

Xml Veri Bağlama bilgilerini temsil eder.

```csharp
public class XmlDataBinding
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Url](../../aspose.cells/xmldatabinding/url/) { get; } | Bu veri bağlamanın kaynak url'sini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellsClassXmlDataBindingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // XML veri bağlamasını kullanacak bir liste nesnesi oluştur.
            ListObject listObject = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 5, 4, true)];

            // XML veri bağlama bilgilerini al (genellikle XML verisi içe aktarılırken ayarlanır).
            XmlDataBinding xmlDataBinding = listObject.XmlMap.DataBinding;

            // XML veri kaynağının URL'sini göster (sadece okunabilir özellik).
            Console.WriteLine("XML Data Binding Source URL: " + xmlDataBinding.Url);

            // Not: Gerçek bir senaryoda, URL XML verisi içe aktarılırken ayarlanır
            // Demonstrasyon amaçlarıyla, özelliğe nasıl erişileceğini gösteriyoruz

            // Çalışma kitabını kaydedin
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


