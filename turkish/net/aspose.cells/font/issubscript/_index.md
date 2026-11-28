---
title: "Font.IsSubscript"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. Yazı tipinin alt simge olup olmadığını belirten bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/font/issubscript/
---
## Font.IsSubscript property

Yazı tipinin alt simge olup olmadığını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IsSubscript { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSubscriptDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Alt simge metniyle bir stil oluştur
            Style subscriptStyle = workbook.CreateStyle();
            subscriptStyle.Font.IsSubscript = true;

            // Karşılaştırma için üst simge metniyle bir stil oluştur
            Style superscriptStyle = workbook.CreateStyle();
            superscriptStyle.Font.IsSuperscript = true;

            // Stilleri hücrelere uygula
            worksheet.Cells["A1"].PutValue("Subscript Text");
            worksheet.Cells["A1"].SetStyle(subscriptStyle);

            worksheet.Cells["A2"].PutValue("Superscript Text");
            worksheet.Cells["A2"].SetStyle(superscriptStyle);

            // Stilleri doğrula ve görüntüle
            Console.WriteLine("A1 IsSubscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A1 IsSuperscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSuperscript);
            Console.WriteLine("A2 IsSubscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A2 IsSuperscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSuperscript);

            // Çalışma kitabını kaydedin
            workbook.Save("FontPropertyIsSubscriptDemo.ods");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


