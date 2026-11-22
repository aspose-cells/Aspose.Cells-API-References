---
title: "SaveOptions.ValidateMergedAreas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SaveOptions. تشير إلى ما إذا كان يجب التحقق من الخلايا المدمجة قبل حفظ الملف"
type: docs
url: /ar/net/aspose.cells/saveoptions/validatemergedareas/
---
## SaveOptions.ValidateMergedAreas property

يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف.

```csharp
public bool ValidateMergedAreas { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyValidateMergedAreasDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين القيم ودمج الخلايا
            worksheet.Cells["A1"].PutValue("Merged Area");
            worksheet.Cells["A2"].PutValue("Test");
            worksheet.Cells.Merge(0, 0, 2, 1); // Merge A1:A2

            // إنشاء خيارات حفظ مع ValidateMergedAreas مضبوط على true
            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                ValidateMergedAreas = true,
                MergeAreas = true
            };

            // حفظ المصنف مع التحقق من المناطق المدمجة
            workbook.Save("ValidateMergedAreasDemo.xlsb", saveOptions);

            Console.WriteLine("Workbook saved with merged areas validation.");
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


