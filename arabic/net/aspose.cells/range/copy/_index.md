---
title: "Range.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. نسخ النطاق مع خيارات اللصق الخاص"
type: docs
url: /ar/net/aspose.cells/range/copy/
---
## Copy(Range, PasteOptions) {#copy_1}

نسخ النطاق باستخدام خيارات اللصق الخاصة.

```csharp
public void Copy(Range range, PasteOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | النطاق | النطاق المصدر. |
| خيارات | PasteOptions | خيارات اللصق الخاص. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangePasteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // إنشاء بيانات عينة في النطاق المصدر
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // إنشاء نطاقات باسم نوع مؤهل بالكامل
            Aspose.Cells.Range source = sheet.Cells.CreateRange(0, 0, 5, 5);
            Aspose.Cells.Range destination = sheet.Cells.CreateRange(6, 0, 5, 5);

            // تعيين خيارات اللصق
            PasteOptions options = new PasteOptions();
            options.PasteType = PasteType.All;

            // نسخ مع خيارات اللصق
            destination.Copy(source, options);

            wb.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PasteOptions](../../pasteoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Range) {#copy}

ينسخ البيانات (بما في ذلك الصيغ)، التنسيق، كائنات الرسم إلخ من نطاق مصدر.

```csharp
public void Copy(Range range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| range | Range | كائن المصدر [`Range`](../). |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // إنشاء نطاقات المصدر والوجهة
            Aspose.Cells.Range sourceRange = cells.CreateRange("A1:A5");
            Aspose.Cells.Range destRange = cells.CreateRange("A6:A10");
            
            // ملء النطاق المصدر ببيانات عينة
            for (int i = 0; i < 5; i++)
            {
                sourceRange[i, 0].PutValue($"Data {i + 1}");
            }
            
            // نسخ النطاق المصدر إلى الوجهة
            sourceRange.Copy(destRange);
            
            workbook.Save("RangeCopyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


