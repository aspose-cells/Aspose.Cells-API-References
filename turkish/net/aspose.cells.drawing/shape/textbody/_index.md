---
title: "Shape.TextBody"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin metin ayarını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/textbody/
---
## Shape.TextBody property

Şeklin metninin ayarını alır ve ayarlar.

```csharp
public FontSettingCollection TextBody { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextBodyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);
            FontSettingCollection fontSettingCollection = shape.TextBody;
            fontSettingCollection.Text = "This is a test.";

            workbook.Save("ShapeTextBodyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSettingCollection](../../../aspose.cells.drawing.texts/fontsettingcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


