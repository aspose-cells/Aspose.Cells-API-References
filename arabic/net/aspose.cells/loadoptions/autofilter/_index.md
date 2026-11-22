---
title: "LoadOptions.AutoFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات"
type: docs
url: /ar/net/aspose.cells/loadoptions/autofilter/
---
## LoadOptions.AutoFilter property

يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات.

```csharp
public bool AutoFilter { get; set; }
```

### ملاحظات

أحيانًا على الرغم من تعيين autofilter، لا يتم إخفاء الصفوف المقابلة في الملف. الآن يعمل فقط لملف SpreadSheetML.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل وتفعيل AutoFilter
            LoadOptions options = new LoadOptions();
            options.AutoFilter = true;

            // تحميل دفتر العمل مع تمكين AutoFilter
            Workbook workbook = new Workbook("example.xlsx", options);

            // الوصول إلى الورقة الأولى وتطبيق AutoFilter
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "A1:D10";
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


