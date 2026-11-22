---
title: "Cell.GetStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحصل على نمط الخلية"
type: docs
url: /ar/net/aspose.cells/cell/getstyle/
---
## GetStyle() {#getstyle}

يحصل على نمط الخلية.

```csharp
public Style GetStyle()
```

### قيمة الإرجاع

كائن النمط.

### ملاحظات

لتغيير نمط الخلية، يرجى استدعاء طريقة Cell.SetStyle() بعد تعديل كائن النمط المُرجع. هذه الطريقة هي نفسها مع `GetStyle` مع قيمة true للمعامل.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين محاذاة رأسية مختلفة للخلايا
            cells["A1"].PutValue("Bottom Alignment");
            cells["A1"].GetStyle().VerticalAlignment = TextAlignmentType.Bottom;

            cells["A2"].PutValue("Center Alignment");
            cells["A2"].GetStyle().VerticalAlignment = TextAlignmentType.Center;

            cells["A3"].PutValue("Distributed Alignment");
            cells["A3"].GetStyle().VerticalAlignment = TextAlignmentType.Distributed;

            cells["A4"].PutValue("Justify Alignment");
            cells["A4"].GetStyle().VerticalAlignment = TextAlignmentType.Justify;

            cells["A5"].PutValue("Top Alignment");
            cells["A5"].GetStyle().VerticalAlignment = TextAlignmentType.Top;

            // عرض طريقة GetStyle()
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("A2 Vertical Alignment: " + cells["A2"].GetStyle().VerticalAlignment);
            Console.WriteLine("A3 Vertical Alignment: " + cells["A3"].GetStyle().VerticalAlignment);
            Console.WriteLine("A4 Vertical Alignment: " + cells["A4"].GetStyle().VerticalAlignment);
            Console.WriteLine("A5 Vertical Alignment: " + cells["A5"].GetStyle().VerticalAlignment);
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetStyle(bool) {#getstyle_1}

إذا كان checkBorders صحيحًا، تحقق مما إذا كانت حدود الخلايا الأخرى ستؤثر على نمط هذه الخلية.

```csharp
public Style GetStyle(bool checkBorders)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| checkBorders | منطقي | تحقق من حدود الخلايا الأخرى |

### قيمة الإرجاع

كائن النمط.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى خلية وتعيين بعض البيانات التجريبية
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(123.456);

            // احصل على نمط الخلية دون وراثته من الصف/العمود (معامل false)
            Style style = cell.GetStyle(false);
            
            // تعديل النمط
            style.Custom = "0.000";
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.None;

            // تطبيق النمط المعدل على الخلية
            cell.SetStyle(style);

            // تحقق من تغييرات النمط
            Console.WriteLine("Number Format: " + cell.GetStyle(false).Custom);
            Console.WriteLine("Top Border Style: " + cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


