---
title: "Name.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Name. تحصل على نص الاسم للكائن"
type: docs
url: /ar/net/aspose.cells/name/text/
---
## Name.Text property

يحصل على نص اسم الكائن.

```csharp
public string Text { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق مسمى
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // تعيين وعرض خاصية Text
            namedRange.Text = "MyCustomName";
            Console.WriteLine("Named range text: " + namedRange.Text);
            
            // احفظ المصنف
            workbook.Save("NamedRangeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


