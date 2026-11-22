---
title: "XlsSaveOptions.MatchColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XlsSaveOptions. تشير إلى ما إذا كان يجب مطابقة لون الخط لأن هناك 56 لونًا في لوحة الألوان القياسية"
type: docs
url: /ar/net/aspose.cells/xlssaveoptions/matchcolor/
---
## XlsSaveOptions.MatchColor property

يشير إلى ما إذا كان يتم مطابقة لون الخط لأن هناك 56 لونًا في لوحة الألوان القياسية.

```csharp
public bool MatchColor { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyMatchColorDemo
    {
        public static void Run()
        {
            // إنشاء مصنف والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى الخلية B2 وتعيين بعض النص بلون خط محدد
            Cell cellB2 = worksheet.Cells["B2"];
            cellB2.PutValue("Sample Text");
            
            // تعيين لون الخط إلى الأزرق
            Style style = cellB2.GetStyle();
            style.Font.Color = Color.Blue;
            cellB2.SetStyle(style);

            // إنشاء خيارات الحفظ مع تعيين MatchColor إلى true
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MatchColor = true;

            // حفظ المصنف باستخدام الخيارات
            workbook.Save("output.xls", saveOptions);

            // إعادة تحميل الملف المحفوظ للتحقق من أن اللون تم الحفاظ عليه
            Workbook savedWorkbook = new Workbook("output.xls");
            Cell savedCellB2 = savedWorkbook.Worksheets[0].Cells["B2"];
            
            // تحقق من أن لون الخط لا يزال أزرق
            Color savedColor = savedCellB2.GetStyle().Font.Color;
            Console.WriteLine("Saved font color: " + savedColor.ToString());
        }
    }
}
```

### انظر أيضًا

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


