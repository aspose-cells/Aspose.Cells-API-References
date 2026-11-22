---
title: "Cell.HasCustomFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. يتحقق مما إذا كان هناك دالة مخصصة غير مدعومة في صيغة هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/hascustomfunction/
---
## Cell.HasCustomFunction property

يتحقق مما إذا كان هناك دالة مخصصة (دالة غير مدعومة) في صيغة هذه الخلية.

```csharp
public bool HasCustomFunction { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook wb = new Workbook();
            
            // أضف اسم دالة مخصصة
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add("MyCustomFunc")].RefersTo = "=MYTESTFUNC()";
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // اختبار باستخدام دالة مدمجة
            Cell cell1 = cells[0, 0];
            cell1.Formula = "=SUM(A1:B1)";
            Console.WriteLine("HasCustomFunction (SUM): " + cell1.HasCustomFunction);
            
            // اختبار باستخدام دالة مخصصة
            Cell cell2 = cells[1, 0];
            cell2.Formula = "=MYTESTFUNC()";
            Console.WriteLine("HasCustomFunction (MYTESTFUNC): " + cell2.HasCustomFunction);
            
            // اختبار باستخدام نطاق مسمى يحتوي على دالة مخصصة
            Cell cell3 = cells[2, 0];
            cell3.Formula = "=MyCustomFunc";
            Console.WriteLine("HasCustomFunction (Named Range): " + cell3.HasCustomFunction);
            
            // اختبار باستخدام دالة مخصصة متداخلة
            Cell cell4 = cells[3, 0];
            cell4.Formula = "=SUM(MYTESTFUNC(), A1)";
            Console.WriteLine("HasCustomFunction (Nested): " + cell4.HasCustomFunction);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


