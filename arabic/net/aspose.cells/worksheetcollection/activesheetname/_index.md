---
title: "WorksheetCollection.ActiveSheetName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تمثل اسم ورقة العمل النشطة عند فتح جدول البيانات"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/activesheetname/
---
## WorksheetCollection.ActiveSheetName property

يمثل اسم ورقة العمل النشطة عند فتح جدول البيانات.

```csharp
public string ActiveSheetName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض أوراق العمل
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // تعيين الورقة النشطة بالاسم
            workbook.Worksheets.ActiveSheetName = "Sheet2";

            // تحقق من الورقة النشطة
            Console.WriteLine("Active Sheet: " + workbook.Worksheets.ActiveSheetName);

            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


