---
title: "WorksheetCollection.IsRefreshAllConnections"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تشير إلى ما إذا كان سيتم تحديث جميع الاتصالات عند فتح الملف في MS Excel"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/isrefreshallconnections/
---
## WorksheetCollection.IsRefreshAllConnections property

يشير إلى ما إذا كان يتم تحديث جميع الاتصالات عند فتح الملف في MS Excel.

```csharp
public bool IsRefreshAllConnections { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyIsRefreshAllConnectionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى مجموعة أوراق العمل
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // أضف بعض أوراق العمل النموذجية
            worksheets.Add("Sheet1");
            worksheets.Add("Sheet2");
            
            // تعيين خاصية IsRefreshAllConnections
            worksheets.IsRefreshAllConnections = true;
            
            // عرض القيمة الحالية لخاصية IsRefreshAllConnections
            Console.WriteLine("IsRefreshAllConnections: " + worksheets.IsRefreshAllConnections);
            
            // احفظ المصنف
            workbook.Save("WorksheetCollectionPropertyIsRefreshAllConnectionsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


