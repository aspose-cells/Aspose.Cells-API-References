---
title: "UnionRange.Hyperlinks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange özelliği. Aralıktaki tüm bağlantıları alır"
type: docs
url: /tr/net/aspose.cells/unionrange/hyperlinks/
---
## UnionRange.Hyperlinks property

Aralıktaki tüm köprüleri alır.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere bazı bağlantılar ekleyin
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://products.aspose.com/cells");
            worksheet.Hyperlinks.Add("C3", 1, 1, "https://docs.aspose.com/cells/net");

            // Bir aralık oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            UnionRange unionRange = range.UnionRanges(new Aspose.Cells.Range[] { range });

            // Aralıktaki köprüleri alın
            Hyperlink[] hyperlinks = unionRange.Hyperlinks;
            Console.WriteLine("Hyperlinks count in range: " + hyperlinks.Length);

            // Her bir bağlantı hakkında bilgiyi göster
            foreach (Hyperlink link in hyperlinks)
            {
                Console.WriteLine("Address: " + link.Address + ", Text: " + link.TextToDisplay);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("HyperlinksDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Hyperlink](../../hyperlink/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


