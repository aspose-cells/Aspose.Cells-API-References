---
title: "Border.ThemeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Border özelliği. Kenarın tema rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/border/themecolor/
---
## Border.ThemeColor property

Kenarlığın tema rengini alır ve ayarlar.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir hücreye eriş ve stilini al
            Style style = worksheet.Cells["A1"].GetStyle();

            // Kenara tema rengini ayarla
            style.Borders[BorderType.BottomBorder].ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Stili hücreye uygulayın
            worksheet.Cells["A1"].SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("BorderThemeColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThemeColor](../../themecolor/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


