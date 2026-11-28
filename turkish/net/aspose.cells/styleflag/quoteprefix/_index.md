---
title: "StyleFlag.QuotePrefix"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Formülü gizleme ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/quoteprefix/
---
## StyleFlag.QuotePrefix property

Formülü gizle ayarı uygulanacak.

```csharp
public bool QuotePrefix { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine erişin ve sayı gibi görünen ancak metin olarak işlenmesi gereken bir değer ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("123456");

            // Bir stil oluşturun ve QuotePrefix'i true olarak ayarlayın
            Style style = workbook.CreateStyle();
            style.QuotePrefix = true;

            // Bir stil bayrağı oluşturun ve QuotePrefix bayrağını etkinleştirin
            StyleFlag flag = new StyleFlag();
            flag.QuotePrefix = true;

            // Stili hücreye ApplyStyle yerine SetStyle kullanarak uygulayın
            cell.SetStyle(style, flag);

            // Mevcut QuotePrefix değerini gösterin
            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);

            // Etkisini görmek için çalışma kitabını kaydedin (değer Excel'de metin olarak işlenecek)
            workbook.Save("PropertyQuotePrefixDemo.xlsx");

            // Şimdi QuotePrefix'i false olarak değiştirelim ve farkı görelim
            style.QuotePrefix = false;
            cell.SetStyle(style, flag);

            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);
            // Karşılaştırmak için farklı bir adla tekrar kaydedin
            workbook.Save("PropertyQuotePrefixDemo_WithoutPrefix.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


