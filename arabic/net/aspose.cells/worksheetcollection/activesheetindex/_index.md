---
title: "WorksheetCollection.ActiveSheetIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/activesheetindex/
---
## WorksheetCollection.ActiveSheetIndex property

يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات.

```csharp
public int ActiveSheetIndex { get; set; }
```

### ملاحظات

فهرس الورقة يبدأ من الصفر.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد يحتوي على 3 أوراق عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // تعيين فهرس الورقة النشطة إلى 1 (الورقة الثانية)
            workbook.Worksheets.ActiveSheetIndex = 1;

            // تحقق من الورقة النشطة
            Console.WriteLine("Active Sheet: " + workbook.Worksheets[workbook.Worksheets.ActiveSheetIndex].Name);

            // احفظ المصنف
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ActiveSheetDemo.xlsx");
            workbook.Save(outputPath);

            Console.WriteLine("File saved to: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


