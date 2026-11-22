---
title: "FindOptions.LookInType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FindOptions. نوع البحث"
type: docs
url: /ar/net/aspose.cells/findoptions/lookintype/
---
## FindOptions.LookInType property

ابحث في النوع.

```csharp
public LookInType LookInType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookInTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف وإضافة بيانات نموذجية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين القيم والصيغ في الخلايا
            worksheet.Cells["A1"].PutValue("SearchValue");
            worksheet.Cells["A2"].Formula = "=A1";
            worksheet.Cells["B1"].PutValue("OtherValue");

            // إنشاء خيارات البحث للبحث فقط في الصيغ
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            // البحث عن القيمة في الصيغ
            Cell foundCell = worksheet.Cells.Find("SearchValue", null, options);

            // أخرج النتيجة.
            if (foundCell != null)
            {
                Console.WriteLine($"Found at: Row {foundCell.Row}, Column {foundCell.Column}");
            }
            else
            {
                Console.WriteLine("Value not found in formulas");
            }
        }
    }
}
```

### انظر أيضًا

* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


