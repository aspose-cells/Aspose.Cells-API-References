---
title: "HtmlSaveOptions.EncodeEntityAsCode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML karakter varlıklarının ondalık kodla değiştirilip değiştirilmeyeceğini gösterir. Örneğin nbsp 160 ile değiştirilir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/encodeentityascode/
---
## HtmlSaveOptions.EncodeEntityAsCode property

HTML karakter varlıklarının ondalık kodla değiştirilip değiştirilmediğini gösterir. (ör. "&amp;nbsp;" "&amp;#160;" ile değiştirilir). Varsayılan değer false'tur.

```csharp
public bool EncodeEntityAsCode { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlSaveOptionsPropertyEncodeEntityAsCodeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel karakterlerle örnek veri ekle
            worksheet.Cells["A1"].PutValue("Sample & Text");
            worksheet.Cells["A2"].PutValue("Another <Test> String");
            worksheet.Cells["A3"].PutValue("Price: $100");

            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions options = new HtmlSaveOptions();

            // EncodeEntityAsCode'un mevcut değerini göster
            Console.WriteLine("Current EncodeEntityAsCode value: " + options.EncodeEntityAsCode);

            // EncodeEntityAsCode'u true olarak ayarla
            options.EncodeEntityAsCode = true;

            // Varlıkları kod olarak kodlanmış şekilde kaydet
            workbook.Save("HtmlWithEncodedEntities.html", options);

            // EncodeEntityAsCode'u false olarak ayarla
            options.EncodeEntityAsCode = false;

            // Varlıkları olduğu gibi kaydet
            workbook.Save("HtmlWithRawEntities.html", options);

            // Çıktı dosyalarını karşılaştır
            Console.WriteLine("Files created:");
            Console.WriteLine("1. HtmlWithEncodedEntities.html - with encoded entities");
            Console.WriteLine("2. HtmlWithRawEntities.html - with raw entities");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


