---
title: "TxtLoadOptions.PreferredParsers"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Metin dosyasını yüklemek için tercih edilen değer ayrıştırıcılarını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/preferredparsers/
---
## TxtLoadOptions.PreferredParsers property

Metin dosyası yükleme için tercih edilen değer ayrıştırıcılarını alır ve ayarlar.

```csharp
public ICustomParser[] PreferredParsers { get; set; }
```

### Açıklamalar

parsers[0] ilk sütun için kullanılacak ayrıştırıcıdır, parsers[1] ikinci sütun için kullanılacak ayrıştırıcıdır, ... vb. Sonuncusu (parsers[parsers.length-1]) parsers.length-1'den başlayan diğer tüm sütunlar için kullanılacaktır. Bir öğe null ise, ilgili sütun Aspose.Cells'ın varsayılan ayrıştırıcısı tarafından ayrıştırılır.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyPreferredParsersDemo
    {
        private class StringParser : ICustomParser
        {
            public bool Parse(string value, out object result)
            {
                result = value; // Always return as string
                return true;
            }

            public object ParseObject(string value)
            {
                return value; // Always return as string
            }

            public string GetFormat()
            {
                return "String"; // Return format description
            }
        }

        public static void Run()
        {
            // CSV yükleme seçeneklerini oluştur
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            
            // Tercih edilen ayrıştırıcıları ayarlayın - önce özel dize ayrıştırıcısını deneyin, ardından varsayılan ayrıştırıcıları
            options.PreferredParsers = new ICustomParser[] { new StringParser(), null };

            // Tarih içeren örnek CSV verisi
            string csvData = "\"2018-10-08\",2018-10-08\n\"2018-10-08\",2018-10-08";
            
            // Seçeneklerle çalışma kitabını yükle
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Cells cells = workbook.Worksheets[0].Cells;

            // Ayrıştırma sonuçlarını doğrulayın
            Console.WriteLine("A1 Type: " + cells[0, 0].Type); // Should be string
            Console.WriteLine("A1 Value: " + cells[0, 0].StringValue); // "2018-10-08"
            Console.WriteLine("B1 Type: " + cells[0, 1].Type); // Should be DateTime
            Console.WriteLine("B1 Value: " + cells[0, 1].DateTimeValue); // 10/8/2018
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


