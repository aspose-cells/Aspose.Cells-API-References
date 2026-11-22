---
title: "Style.Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ Style. يهيئ نسخة جديدة من الفئة Style"
type: docs
url: /ar/net/aspose.cells/style/style/
---
## Style constructor

يهيئ نسخة جديدة من الفئة [`Style`](../).

```csharp
[Obsolete("Use CellsFactory.CreateStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style()
```

### ملاحظات

ملاحظة: هذا المنشئ أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام طريقة CellsFactory.CreateStyle(). سيتم إزالة هذه الخاصية بعد 6 أشهر منذ أكتوبر 2016. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط باستخدام المنشئ
            Style style = new Style();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;

            // تطبيق النمط على خلية
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Text");
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("StyleConstructorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


