---
title: "FormatConditionCollection.GetCellArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FormatConditionCollection. يحصل على نطاق الخلية المُنسَّقة شرطياً حسب الفهرس"
type: docs
url: /ar/net/aspose.cells/formatconditioncollection/getcellarea/
---
## FormatConditionCollection.GetCellArea method

يحصل على نطاق الخلايا المُنسق شرطياً حسب الفهرس.

```csharp
public CellArea GetCellArea(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس نطاق الخلية المُنسَّقة شرطياً. |

### قيمة الإرجاع

نطاق الخلية المُنسَّقة شرطياً

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodGetCellAreaWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = i + j;
                }
            }

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // تحديد نطاق التنسيق الشرطي
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 7;
            area.EndColumn = 3;
            fcc.AddArea(area);

            // إضافة شرط وتعيين النمط
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "10");
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            fcc[conditionIndex].Style = style;

            // الحصول على معلومات مساحة الخلية وعرضها
            CellArea retrievedArea = fcc.GetCellArea(0);
            Console.WriteLine("Conditional Format Area:");
            Console.WriteLine($"StartRow: {retrievedArea.StartRow}");
            Console.WriteLine($"StartColumn: {retrievedArea.StartColumn}");
            Console.WriteLine($"EndRow: {retrievedArea.EndRow}");
            Console.WriteLine($"EndColumn: {retrievedArea.EndColumn}");

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


