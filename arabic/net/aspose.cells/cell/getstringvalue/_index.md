---
title: "Cell.GetStringValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. يحصل على قيمة السلسلة وفق استراتيجية تنسيق محددة"
type: docs
url: /ar/net/aspose.cells/cell/getstringvalue/
---
## Cell.GetStringValue method

يحصل على قيمة السلسلة باستخدام استراتيجية تنسيق محددة.

```csharp
public string GetStringValue(CellValueFormatStrategy formatStrategy)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| formatStrategy | CellValueFormatStrategy | استراتيجية التنسيق. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStringValueWithCellValueFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // حدد أنواعًا مختلفة من البيانات في الخلايا
            cells["A1"].PutValue(123.45); // Numeric value
            cells["A2"].PutValue(DateTime.Now); // DateTime value
            cells["A3"].PutValue(true); // Boolean value
            cells["A4"].PutValue("Sample Text"); // String value

            // عرض GetStringValue مع استراتيجيات تنسيق مختلفة
            Console.WriteLine("None: " + cells["A1"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("CellStyle: " + cells["A1"].GetStringValue(CellValueFormatStrategy.CellStyle));
            Console.WriteLine("DisplayString: " + cells["A1"].GetStringValue(CellValueFormatStrategy.DisplayString));

            Console.WriteLine("DateTime None: " + cells["A2"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("DateTime CellStyle: " + cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle));
        }
    }
}
```

### انظر أيضًا

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


