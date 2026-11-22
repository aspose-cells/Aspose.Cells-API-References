---
title: "FontConfigs.DefaultFontName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontConfigs. تحصل أو تعين اسم الخط الافتراضي"
type: docs
url: /ar/net/aspose.cells/fontconfigs/defaultfontname/
---
## FontConfigs.DefaultFontName property

يحصل أو يعيّن اسم الخط الافتراضي.

```csharp
public static string DefaultFontName { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // عرض اسم الخط الافتراضي الحالي
            Console.WriteLine("Current DefaultFontName value: " + FontConfigs.DefaultFontName);

            // تعيين اسم خط افتراضي جديد
            FontConfigs.DefaultFontName = "Arial";

            // إنشاء نمط بدون تحديد خط صريح لتوضيح استخدام الخط الافتراضي
            Style style = workbook.CreateStyle();
            style.Font.Name = ""; // Empty to use default font

            // تطبيق النمط على خلية
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text should use the default font");
            cell.SetStyle(style);

            // حفظ المصنف لرؤية التأثير
            workbook.Save("PropertyDefaultFontNameDemo.xlsx");

            // تحقق من تطبيق الخط بشكل صحيح
            Console.WriteLine("Cell font after setting DefaultFontName: " + cell.GetStyle().Font.Name);
        }
    }
}
```

### انظر أيضًا

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


