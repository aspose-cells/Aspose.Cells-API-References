---
title: "Column.Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Column. تحصل على النمط لهذا العمود"
type: docs
url: /ar/net/aspose.cells/column/style/
---
## Column.Style property

يحصل على نمط هذا العمود.

```csharp
[Obsolete("Use Column.GetStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style Style { get; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة Column.GetStyle() للحصول على النمط الافتراضي لهذا العمود. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى العمود الأول
            Column column = worksheet.Cells.Columns[0];
            
            // احصل على النمط الحالي باستخدام خاصية Style
            Style originalStyle = column.Style;
            Console.WriteLine("Original column style - Background: " + originalStyle.BackgroundColor);
            
            // إنشاء نمط جديد وتعديل الخصائص
            Style newStyle = workbook.CreateStyle();
            newStyle.BackgroundColor = Color.LightBlue;
            newStyle.Font.IsBold = true;
            newStyle.HorizontalAlignment = TextAlignmentType.Center;
            
            // تطبيق النمط الجديد على العمود
            column.SetStyle(newStyle);
            
            // إضافة بيانات لتوضيح تطبيق النمط
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // تحقق من تغييرات النمط
            Console.WriteLine("New column style applied - Background: " + column.GetStyle().BackgroundColor);
            
            // حفظ مع تعديل عرض العمود
            column.Width = 15;
            workbook.Save("ColumnStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


