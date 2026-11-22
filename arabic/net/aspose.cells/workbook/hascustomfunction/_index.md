---
title: "Workbook.HasCustomFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تكشف ما إذا كان هناك دالة مخصصة مستخدمة في هذا المصنف مثل في صيغ الخلايا في الأسماء المعرفة"
type: docs
url: /ar/net/aspose.cells/workbook/hascustomfunction/
---
## Workbook.HasCustomFunction property

يكشف ما إذا كان هناك دالة مخصصة مستخدمة في هذا المصنف، مثل في صيغة الخلية أو في الأسماء المعرفة...

```csharp
public bool HasCustomFunction { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // إضافة صيغة قياسية إلى اسم
            NameCollection names = wb.Worksheets.Names;
            int index = names.Add("StandardName");
            names[index].RefersTo = "=SUM(Sheet1!$A$1:$A$2)";
            Console.WriteLine($"Workbook has custom function (should be false): {wb.HasCustomFunction}");

            // إضافة دالة مخصصة إلى اسم
            index = names.Add("CustomName");
            names[index].RefersTo = "=MYFUNC()";
            Console.WriteLine($"Workbook has custom function (should be true): {wb.HasCustomFunction}");

            // اختبار باستخدام صيغ الخلايا
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // دالة قياسية في الخلية
            cells["A1"].Formula = "=SUM(B1:B2)";
            Console.WriteLine($"Cell has custom function (should be false): {cells["A1"].HasCustomFunction}");

            // دالة مخصصة في الخلية
            cells["A2"].Formula = "=MYFUNC(B1)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A2"].HasCustomFunction}");

            // إشارة إلى اسم مع دالة مخصصة
            cells["A3"].Formula = "=CustomName";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A3"].HasCustomFunction}");

            // دوال مخصصة مركبة
            cells["A4"].Formula = "=MYFUNC(CustomName)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A4"].HasCustomFunction}");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


