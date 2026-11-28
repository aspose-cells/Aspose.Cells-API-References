---
title: "Font.ThemeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Yazı tipi özelliği. Tema rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/font/themecolor/
---
## Font.ThemeColor property

Tema rengini alır ve ayarlar.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Açıklamalar

Yazı tipi rengi bir tema rengi değilse, NULL döndürülecektir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine eriş ve metni ayarla
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Color Demo");

            // Stili ve yazı tipini al
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Tema rengi oluştur ve ayarla
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

            // Stili hücreye uygulayın
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("ThemeColorDemo.xlsx");

            // Tema rengini doğrula
            Font savedFont = worksheet.Cells["A1"].GetStyle().Font;
            Console.WriteLine("ThemeColor Type: " + savedFont.ThemeColor.ColorType);
            Console.WriteLine("ThemeColor Tint: " + savedFont.ThemeColor.Tint);
        }
    }
}
```

### Ayrıca Bakınız

* class [ThemeColor](../../themecolor/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


