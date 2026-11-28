---
title: "FontSettingCollection.TextAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSettingCollection özelliği. Metin gövdesinin hizalama ayarını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/fontsettingcollection/textalignment/
---
## FontSettingCollection.TextAlignment property

Metin gövdesinin hizalama ayarını temsil eder.

```csharp
public ShapeTextAlignment TextAlignment { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyTextAlignmentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            shape.Text = "Sample Text";

            // TextAlignment özelliklerine erişin ve değiştirin
            var textAlignment = shape.TextBody.TextAlignment;
            
            Console.WriteLine("Default Margins (Points):");
            Console.WriteLine($"AutoMargin: {textAlignment.IsAutoMargin}");
            Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
            Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
            Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
            Console.WriteLine($"Right: {textAlignment.RightMarginPt}");

            // Kenar boşluklarını değiştirin
            textAlignment.TopMarginPt = 36;
            textAlignment.BottomMarginPt = 36;
            textAlignment.LeftMarginPt = 18;
            textAlignment.RightMarginPt = 18;

            // Çalışma kitabını kaydedin
            workbook.Save("TextAlignmentDemo.xlsx");

            Console.WriteLine("\nModified Margins (Points):");
            Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
            Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
            Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
            Console.WriteLine($"Right: {textAlignment.RightMarginPt}");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeTextAlignment](../../shapetextalignment/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


