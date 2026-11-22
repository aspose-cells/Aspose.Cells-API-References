---
title: "Worksheet.VisibilityType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تشير إلى الحالة المرئية لهذه الورقة"
type: docs
url: /ar/net/aspose.cells/worksheet/visibilitytype/
---
## Worksheet.VisibilityType property

يشير إلى الحالة المرئية لهذه الورقة.

```csharp
public VisibilityType VisibilityType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVisibilityTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف أوراق عمل
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // عيّن أنواع رؤية مختلفة لكل ورقة عمل
            workbook.Worksheets[0].VisibilityType = VisibilityType.Hidden;
            workbook.Worksheets[1].VisibilityType = VisibilityType.VeryHidden;
            workbook.Worksheets[2].VisibilityType = VisibilityType.Visible;

            // احفظ المصنف
            string outputPath = "output_visibility.xlsx";
            workbook.Save(outputPath);

            // أعد تحميل دفتر العمل للتحقق من إعدادات الرؤية
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // إخراج أنواع الرؤية
            Console.WriteLine("Worksheet 0 Visibility: " + loadedWorkbook.Worksheets[0].VisibilityType);
            Console.WriteLine("Worksheet 1 Visibility: " + loadedWorkbook.Worksheets[1].VisibilityType);
            Console.WriteLine("Worksheet 2 Visibility: " + loadedWorkbook.Worksheets[2].VisibilityType);
        }
    }
}
```

### انظر أيضًا

* enum [VisibilityType](../../visibilitytype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


