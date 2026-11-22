---
title: "FormatConditionCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FormatConditionCollection. تضيف شرط تنسيق ونطاق الخلايا المتأثرة إلى FormatConditions. يمكن أن تحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية. لا يُسمح بالإشارات إلى الأوراق الأخرى في صيغ التنسيق الشرطي"
type: docs
url: /ar/net/aspose.cells/formatconditioncollection/add/
---
## FormatConditionCollection.Add method

يضيف شرط تنسيق ونطاق الخلايا المتأثر إلى FormatConditions. يمكن أن تحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية. لا يُسمح بالإشارات إلى الأوراق الأخرى في صيغ التنسيق الشرطي.

```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType, 
    string formula1, string formula2)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | CellArea | نطاق خلايا مُنسق شرطياً. |
| type | FormatConditionType | نوع التنسيق الشرطي. يمكن أن يكون أحد أعضاء FormatConditionType. |
| operatorType | OperatorType | عامل المقارنة. يمكن أن يكون أحد أعضاء OperatorType. |
| formula1 | String | القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| formula2 | String | القيمة أو التعبير المرتبط بالتنسيق الشرطي |

### قيمة الإرجاع

[0]:Formatting condition object index;[1] Effected cell rang index.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddWithCellAreaFormatConditionTypeOpeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // ملء بيانات عينة
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // إضافة تنسيق شرطي
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            
            // عرض طريقة Add مع المعلمات المحددة
            fcc.Add(
                CellArea.CreateCellArea(0, 0, 4, 0),
                FormatConditionType.Expression,
                OperatorType.None,
                "=A1>AVERAGE(OFFSET($A$1:$A$5,0,0)-0)",
                null
            );

            // تطبيق التنسيق
            int fontSize = wb.DefaultStyle.Font.Size;
            fcc[0].Style.Font.Size = fontSize + 2;

            // احفظ المصنف لعرض النتيجة
            wb.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


