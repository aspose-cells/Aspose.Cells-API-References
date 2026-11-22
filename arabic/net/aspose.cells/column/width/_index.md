---
title: "Column.Width"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Column. تحصل وتضبط عرض العمود بوحدة الأحرف"
type: docs
url: /ar/net/aspose.cells/column/width/
---
## Column.Width property

يحصل على ويضبط عرض العمود بوحدة الأحرف.

```csharp
public double Width { get; set; }
```

### ملاحظات

في جداول البيانات، يُقاس عرض العمود بعدد الأحرف لعرض الرقم الأقصى للأرقام 0~9 كما يُظهره خط النمط العادي.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين العرض للعمود 3 (الفهرس 2)
            worksheet.Cells.Columns[2].Width = 25.5;
            
            // تعيين العرض للعمود 4 (الفهرس 3)
            worksheet.Cells.Columns[3].Width = 40.0;
            
            // احصل على الأعرض وعرضها
            Console.WriteLine("Column 3 Width: " + worksheet.Cells.Columns[2].Width);
            Console.WriteLine("Column 4 Width: " + worksheet.Cells.Columns[3].Width);
            
            // احفظ المصنف
            workbook.Save("ColumnWidthDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


