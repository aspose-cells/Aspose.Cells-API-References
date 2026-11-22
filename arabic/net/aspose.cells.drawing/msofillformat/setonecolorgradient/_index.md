---
title: "MsoFillFormat.SetOneColorGradient"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة MsoFillFormat. تعيّن الملء المحدد إلى تدرّج لون واحد"
type: docs
url: /ar/net/aspose.cells.drawing/msofillformat/setonecolorgradient/
---
## MsoFillFormat.SetOneColorGradient method

تعيين الملء المحدد إلى تدرج لون واحد.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اللون | اللون | لون تدرج واحد. |
| درجة | Double | درجة التدرج. يمكن أن تكون قيمة من 0.0 (غامق) إلى 1.0 (فاتح). |
| النمط | GradientStyleType | نمط تظليل التدرج. |
| variant | Int32 | متغير التدرج. يمكن أن يكون قيمة من 1 إلى 4، المقابل لأحد المتغيرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان style هو GradientStyle.FromCenter، فإن معامل Variant لا يمكن أن يكون إلا 1 أو 2. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 50, 50);
            MsoFillFormat fillFormat = shape.FillFormat;

            // تعيين تدرّج لون واحد باستخدام المعلمات المحددة
            fillFormat.SetOneColorGradient(Color.Red, 0.5, GradientStyleType.DiagonalUp, 2);

            workbook.Save("GradientFillExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


