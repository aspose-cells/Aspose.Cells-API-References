---
title: "FormatConditionCollection.AddArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FormatConditionCollection. تضيف نطاق خلية مُنسَّقة شرطياً"
type: docs
url: /ar/net/aspose.cells/formatconditioncollection/addarea/
---
## FormatConditionCollection.AddArea method

يضيف نطاق خلايا مُنسق شرطياً.

```csharp
public int AddArea(CellArea cellArea)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | CellArea | نطاق خلايا مُنسق شرطياً. |

### قيمة الإرجاع

فهرس نطاق الخلية المُنسَّقة شرطياً.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue(row * col);
                }
            }

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection formatCollection = worksheet.ConditionalFormattings[index];
            
            // أنشئ شرط تنسيق
            formatCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // إنشاء مساحات خلايا وإضافتها إلى مجموعة التنسيق
            CellArea area1 = CellArea.CreateCellArea(0, 0, 4, 4);
            CellArea area2 = CellArea.CreateCellArea(5, 5, 9, 9);
            
            formatCollection.AddArea(area1);
            formatCollection.AddArea(area2);

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


