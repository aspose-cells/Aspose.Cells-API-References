---
title: "Style.Font"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Bir Font nesnesi alır"
type: docs
url: /tr/net/aspose.cells/style/font/
---
## Style.Font property

`Font` nesnesi alır.

```csharp
public Font Font { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // B4 hücresine eriş ve yazı tipini kalın yap
            Cell b4 = cells["B4"];
            Style b4Style = b4.GetStyle();
            b4Style.Font.IsBold = true;
            b4.SetStyle(b4Style);

            // C4 hücresine eriş ve yazı tipinin kalın olmadığından emin ol
            Cell c4 = cells["C4"];
            Style c4Style = c4.GetStyle();
            c4Style.Font.IsBold = false;
            c4.SetStyle(c4Style);

            // D4 hücresine eriş ve yazı tipini farklı bir renkle kalın yap
            Cell d4 = cells["D4"];
            Style d4Style = d4.GetStyle();
            d4Style.Font.IsBold = true;
            d4Style.Font.Color = Color.Red;
            d4.SetStyle(d4Style);

            // Yazı tipi özelliklerini doğrula
            Console.WriteLine("B4 Font Bold: " + b4.GetStyle().Font.IsBold);
            Console.WriteLine("C4 Font Bold: " + c4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Bold: " + d4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Color: " + d4.GetStyle().Font.Color);

            // Çalışma kitabını kaydedin
            workbook.Save("FontPropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../../font/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


