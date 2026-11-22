---
title: "Cells.PreserveString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل أو تحدد قيمة تشير إلى ما إذا كانت جميع قيم ورقة العمل محفوظة كسلاسل. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/cells/preservestring/
---
## Cells.PreserveString property

يحصل أو يعيّن قيمة تشير إلى ما إذا كانت جميع قيم ورقة العمل محفوظة كسلاسل. القيمة الافتراضية هي false.

```csharp
public bool PreserveString { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyPreserveStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // قم بتعيين خاصية PreserveString إلى true
            cells.PreserveString = true;

            // إضافة قيم نصية إلى الخلايا
            cells["A1"].PutValue("Preserved String 1");
            cells["B1"].PutValue("Preserved String 2");

            // الوصول إلى القيم (سيتم حفظها كسلاسل)
            Console.WriteLine("Cell A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + cells["B1"].StringValue);

            // احفظ المصنف
            workbook.Save("PreserveStringDemo.xlsx", SaveFormat.Xlsx);

            // تحميل المصنف المحفوظ للتحقق من الحفظ
            Workbook loadedWorkbook = new Workbook("PreserveStringDemo.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;

            // إخراج القيم المحفوظة
            Console.WriteLine("\nAfter loading:");
            Console.WriteLine("Cell A1 value: " + loadedCells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + loadedCells["B1"].StringValue);

            // عرض مقارنة خاصية PreserveString
            Console.WriteLine("\nPreserveString property matches: " + 
                (cells.PreserveString == loadedCells.PreserveString));
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


