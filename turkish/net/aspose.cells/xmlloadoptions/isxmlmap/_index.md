---
title: "XmlLoadOptions.IsXmlMap"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlLoadOptions özelliği. XML'in Excel'e eşlenip eşlenmediğini gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/xmlloadoptions/isxmlmap/
---
## XmlLoadOptions.IsXmlMap property

XML'nin Excel'e eşlenip eşlenmediğini gösterir. Varsayılan değer false'tur.

```csharp
public bool IsXmlMap { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIsXmlMapDemo
    {
        public static void Run()
        {
            // XmlLoadOptions sınıfının bir örneğini oluştur.
            XmlLoadOptions options = new XmlLoadOptions();

            // Dosya yüklenirken XML eşlemesini etkinleştirin
            options.IsXmlMap = true;

            // Belirtilen seçenekleri kullanarak bir XML dosyasını Çalışma Kitabı'na yükle.
            Workbook workbook = new Workbook("sample.xml", options);

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Yüklenen XML'den bazı verileri göstererek başarılı eşlemeyi gösterin
            Console.WriteLine("Data from loaded XML:");
            Console.WriteLine(worksheet.Cells["A1"].StringValue);
            Console.WriteLine(worksheet.Cells["A2"].StringValue);

            // Çalışma kitabını yeni bir Excel dosyasına kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


