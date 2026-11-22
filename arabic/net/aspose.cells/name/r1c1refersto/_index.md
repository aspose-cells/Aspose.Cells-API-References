---
title: "Name.R1C1RefersTo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Name. تحصل أو تعين مرجع R1C1 للـ Name"
type: docs
url: /ar/net/aspose.cells/name/r1c1refersto/
---
## Name.R1C1RefersTo property

يحصل أو يعين مرجع R1C1 للـ [`Name`](../).

```csharp
public string R1C1RefersTo { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyR1C1RefersToDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة اسم جديد إلى مجموعة الأسماء
            int nameIndex = workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names[nameIndex];
            
            // تعيين مرجع R1C1 للاسم
            name.R1C1RefersTo = "'Sheet1'!R3C1:R9C4";
            
            // تحقق من أن المرجع تم تعيينه بشكل صحيح
            Console.WriteLine("Name refers to: " + name.RefersTo);
            
            // احفظ المصنف
            workbook.Save("NamePropertyR1C1RefersToDemo_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


