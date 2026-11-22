---
title: "SaveOptions.SortNames"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SaveOptions. تشير إلى ما إذا كان سيتم فرز الأسماء المعرفة قبل حفظ الملف"
type: docs
url: /ar/net/aspose.cells/saveoptions/sortnames/
---
## SaveOptions.SortNames property

يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف.

```csharp
public bool SortNames { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySortNamesDemo
    {
        public static void Run()
        {
            // إنشاء كائن Workbook جديد
            Workbook workbook = new Workbook();
            
            // أضف بيانات تجريبية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // إنشاء نطاق مسمى
            worksheet.Cells.CreateRange("A2:B3").Name = "MyDataRange";

            // إنشاء خيارات الحفظ مع تمكين SortNames enabled
            XlsSaveOptions saveOptions = new XlsSaveOptions
            {
                SortNames = true
            };

            // احفظ المصنف
            workbook.Save("SortedNamesExample.xls", saveOptions);

            Console.WriteLine("Workbook saved with sorted named ranges.");
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


