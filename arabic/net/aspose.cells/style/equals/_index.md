---
title: "Style.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Style. تحدد ما إذا كان كائنان من Style متساويين"
type: docs
url: /ar/net/aspose.cells/style/equals/
---
## Style.Equals method

يحدد ما إذا كان كائني Style متساويين.

```csharp
public override bool Equals(object obj)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | Object | كائن Style للمقارنة مع كائن Style الحالي. |

### قيمة الإرجاع

صحيح إذا كان الكائن المحدد مساويًا للكائن الحالي؛ وإلا، خطأ.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمطين للمقارنة
            Style style1 = workbook.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.HorizontalAlignment = TextAlignmentType.Center;

            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Arial";
            style2.Font.Size = 12;
            style2.HorizontalAlignment = TextAlignmentType.Center;

            try
            {
                // استدعاء طريقة Equals لمقارنة الأنماط
                bool areEqual = style1.Equals((object)style2);

                // اعرض النتيجة
                Console.WriteLine($"The styles are equal: {areEqual}");

                // تطبيق الأنماط لإظهار أنها متطابقة
                if (areEqual)
                {
                    Cell cell1 = worksheet.Cells["A1"];
                    cell1.PutValue("Style 1");
                    cell1.SetStyle(style1);

                    Cell cell2 = worksheet.Cells["A2"];
                    cell2.PutValue("Style 2");
                    cell2.SetStyle(style2);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("StyleEqualsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


