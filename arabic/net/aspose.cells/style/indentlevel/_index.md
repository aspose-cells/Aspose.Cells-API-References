---
title: "Style.IndentLevel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تمثل مستوى المسافة البادئة للخلية أو النطاق. يمكن أن تكون عددًا صحيحًا فقط من 0 إلى 250"
type: docs
url: /ar/net/aspose.cells/style/indentlevel/
---
## Style.IndentLevel property

يمثل مستوى المسافة البادئة للخلية أو النطاق. يمكن أن يكون عددًا صحيحًا فقط من 0 إلى 250.

```csharp
public int IndentLevel { get; set; }
```

### ملاحظات

إذا تم تعيين نوع محاذاة النص الأفقي إلى قيمة غير اليسار أو اليمين، سيتم إعادة مستوى المسافة البادئة إلى الصفر.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIndentLevelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين مستويات مسافة بادئة مختلفة للخلايا
            for (int i = 0; i < 16; i++)
            {
                Cell cell = cells[i, 0];
                Style style = cell.GetStyle();
                style.IndentLevel = i;
                style.HorizontalAlignment = TextAlignmentType.Left;
                cell.SetStyle(style);
                cell.PutValue($"Indent Level {i}");
            }

            // احفظ المصنف
            workbook.Save("IndentLevelDemo.xlsx");
            Console.WriteLine("Workbook saved with different indent levels.");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


