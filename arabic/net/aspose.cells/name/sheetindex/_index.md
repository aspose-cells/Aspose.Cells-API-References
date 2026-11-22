---
title: "Name.SheetIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Name. تشير إلى أن هذا الاسم ينتمي إلى Workbook أو Worksheet. 0 اسم عام وإلا فالمؤشر إلى الورقة يبدأ من الواحد"
type: docs
url: /ar/net/aspose.cells/name/sheetindex/
---
## Name.SheetIndex property

يشير إلى أن هذا الاسم ينتمي إلى مصنف Workbook أو ورقة Worksheet. 0 = اسم عالمي، وإلا فالمؤشر إلى الورقة (مؤشر يبدأ من 1).

```csharp
public int SheetIndex { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertySheetIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض أوراق العمل
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // إنشاء نطاق مسمى في Sheet2
            Worksheet sheet2 = workbook.Worksheets["Sheet2"];
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet2!$A$1:$B$10";
            
            // عرض فهرس الورقة للنطاق المسمى
            Console.WriteLine("Sheet index of named range: " + name.SheetIndex);
            
            // احفظ المصنف
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


