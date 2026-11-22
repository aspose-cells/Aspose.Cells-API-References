---
title: "Style.IsBorderApplied"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تشير إلى ما إذا كان يجب تطبيق تنسيق الحدود"
type: docs
url: /ar/net/aspose.cells/style/isborderapplied/
---
## Style.IsBorderApplied property

يشير إلى ما إذا كان يجب تطبيق تنسيق الحدود.

```csharp
public bool IsBorderApplied { get; set; }
```

### ملاحظات

فقط للنمط المسمى.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsBorderAppliedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نمط مخصص
            Style style = workbook.CreateStyle();
            
            // تطبيق إعدادات الحدود على النمط
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Black;
            
            // تحقق مما إذا تم تطبيق الحدود
            Console.WriteLine("IsBorderApplied before setting: " + style.IsBorderApplied);
            
            // قم بتعيين IsBorderApplied صراحةً إلى true
            style.IsBorderApplied = true;
            
            // تطبيق النمط على خلية
            worksheet.Cells["A1"].SetStyle(style);
            
            // تحقق من تطبيق الحدود
            Console.WriteLine("IsBorderApplied after setting: " + style.IsBorderApplied);
            
            // احفظ المصنف
            workbook.Save("IsBorderAppliedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


