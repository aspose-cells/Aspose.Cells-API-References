---
title: "PasteOptions.OnlyVisibleCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PasteOptions. True يعني نسخ الخلايا المرئية فقط"
type: docs
url: /ar/net/aspose.cells/pasteoptions/onlyvisiblecells/
---
## PasteOptions.OnlyVisibleCells property

True يعني نسخ الخلايا المرئية فقط.

```csharp
public bool OnlyVisibleCells { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOnlyVisibleCellsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف يحتوي على ورقتي عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // الحصول على الخلايا من ورقة العمل الأولى وتعبئة البيانات
            Cells sourceCells = workbook.Worksheets[0].Cells;
            sourceCells["A1"].PutValue("Hidden A1");
            sourceCells["B2"].PutValue("Visible B2");
            sourceCells["C3"].PutValue("Hidden C3");
            
            // إخفاء بعض الصفوف والأعمدة
            sourceCells.HideRow(0);  // Hides row 1 (A1)
            sourceCells.HideColumn(2); // Hides column C (C3)

            // إنشاء نطاق المصدر للنسخ
            Aspose.Cells.Range sourceRange = sourceCells.CreateRange("A1:C3");
            
            // الحصول على الخلايا من ورقة العمل الثانية للوجهة
            Cells destCells = workbook.Worksheets[1].Cells;
            Aspose.Cells.Range destRange = destCells.CreateRange("A1:C3");
            
            // إنشاء خيارات اللصق وتعيين OnlyVisibleCells
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.OnlyVisibleCells = true;
            
            // نسخ الخلايا المرئية فقط
            destRange.Copy(sourceRange, pasteOptions);
            
            // إخراج النتائج لتوضيح الوظيفة
            Console.WriteLine("B2 value (should be copied): " + destCells["B2"].StringValue);
            Console.WriteLine("A1 value (should be empty): " + destCells["A1"].StringValue);
            Console.WriteLine("C3 value (should be empty): " + destCells["C3"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


