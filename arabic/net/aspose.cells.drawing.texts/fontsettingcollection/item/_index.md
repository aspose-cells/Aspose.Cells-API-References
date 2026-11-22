---
title: "FontSettingCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontSettingCollection. تحصل على FontSetting حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.drawing.texts/fontsettingcollection/item/
---
## FontSettingCollection indexer

تحصل على [`FontSetting`](../../../aspose.cells/fontsetting/) حسب الفهرس.

```csharp
public FontSetting this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook w = new Workbook();
            Worksheet s = w.Worksheets[0];

            Shape tb = s.Shapes.AddTextBox(3, 0, 7, 0, 70, 300);
            tb.Text = "Sample Text";

            // تعيين خصائص الخط للأحرف المحددة
            Aspose.Cells.Font fo = tb.Characters(3, 5).Font;
            fo.IsSuperscript = true;
            fo.Color = Color.Red;

            // الوصول إلى الخط عبر خاصية TextBody.Item
            Aspose.Cells.Font fo1 = tb.TextBody[3].Font;
            Console.WriteLine("IsSuperscript: " + fo1.IsSuperscript);
            Console.WriteLine("Color: " + fo1.Color);

            w.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


