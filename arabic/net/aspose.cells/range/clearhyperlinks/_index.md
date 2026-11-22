---
title: "Range.ClearHyperlinks"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. يزيل الروابط فقط"
type: docs
url: /ar/net/aspose.cells/range/clearhyperlinks/
---
## Range.ClearHyperlinks method

يزيل الروابط التشعبية فقط.

```csharp
public void ClearHyperlinks(bool clearFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| clearFormat | منطقي | تشير إلى ما إذا كان يجب مسح تنسيق الروابط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearHyperlinksWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق وإضافة بعض الروابط للتوضيح
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");
            range.AddHyperlink("https://www.example.com", "Example", "Visit Example");

            try
            {
                // مسح الروابط التشعبية مع الحفاظ على التنسيق (false)
                range.ClearHyperlinks(false);
                Console.WriteLine("Hyperlinks cleared while preserving format");

                // إضافة الروابط التشعبية مرة أخرى
                range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");

                // مسح الروابط التشعبية دون الحفاظ على التنسيق (true)
                range.ClearHyperlinks(true);
                Console.WriteLine("Hyperlinks cleared without preserving format");

                // احفظ المصنف
                workbook.Save("ClearHyperlinksDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


