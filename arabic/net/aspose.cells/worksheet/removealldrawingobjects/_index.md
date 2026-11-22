---
title: "Worksheet.RemoveAllDrawingObjects"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تزيل جميع كائنات الرسم في هذه الورقة"
type: docs
url: /ar/net/aspose.cells/worksheet/removealldrawingobjects/
---
## Worksheet.RemoveAllDrawingObjects method

يزيل جميع كائنات الرسم في هذه ورقة العمل.

```csharp
public void RemoveAllDrawingObjects()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAllDrawingObjectsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض كائنات الرسم إلى الورقة
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);
            worksheet.Shapes.AddLine(1, 0, 5, 100, 5, 150);
            
            // احفظ قبل إزالة الكائنات
            workbook.Save("BeforeRemove.xlsx", SaveFormat.Xlsx);
            
            // إزالة جميع كائنات الرسم
            worksheet.RemoveAllDrawingObjects();
            
            // احفظ بعد إزالة الكائنات
            workbook.Save("AfterRemove.xlsx", SaveFormat.Xlsx);
            
            // تخلص من المصنف
            workbook.Dispose();
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


