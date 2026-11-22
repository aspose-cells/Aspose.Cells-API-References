---
title: "FormatConditionCollection.RemoveArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FormatConditionCollection. تُزيل نطاق الخلايا المُنسَّق شرطيًا حسب الفهرس"
type: docs
url: /ar/net/aspose.cells/formatconditioncollection/removearea/
---
## RemoveArea(int) {#removearea_1}

يزيل نطاق الخلايا المُنسق شرطياً حسب الفهرس.

```csharp
public void RemoveArea(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس نطاق الخلايا المُنسَّق شرطيًا الذي سيتم إزالته. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تنسيق شرطي
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];

            // إضافة مناطق للتنسيق
            formatConditionCollection.AddArea(CellArea.CreateCellArea(0, 0, 10, 5)); // First area
            formatConditionCollection.AddArea(CellArea.CreateCellArea(5, 5, 15, 10)); // Second area

            // إضافة شرط
            formatConditionCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");

            // عرض عدد المناطق الأولي (نعلم أننا أضفنا منطقتين)
            Console.WriteLine("Areas before removal: 2");

            // إزالة المنطقة الثانية (الفهرس 1)
            formatConditionCollection.RemoveArea(1);

            // عرض عدد المناطق بعد الإزالة (نعلم أننا أزلنا منطقة واحدة)
            Console.WriteLine("Areas after removal: 1");

            // احفظ المصنف
            workbook.Save("RemoveAreaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveArea(int, int, int, int) {#removearea}

إزالة التنسيق الشرطي في النطاق.

```csharp
public bool RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | الـ startRow للنطاق. |
| startColumn | Int32 | الـ startColumn للنطاق. |
| totalRows | Int32 | عدد الصفوف في النطاق. |
| totalColumns | Int32 | عدد الأعمدة في النطاق. |

### قيمة الإرجاع

يرجع TRUE، يجب إزالة هذا FormatCondtionCollection.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            
            int idx = cfc.Add();
            FormatConditionCollection fcc = cfc[idx];
            
            // إضافة المنطقة الأولية
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            fcc.AddArea(initialArea);
            
            // إضافة شرط
            idx = fcc.AddCondition(FormatConditionType.Expression);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "=A1>0";
            fc.Style.Font.Color = Color.Red;
            
            // عرض RemoveArea مع معلمات Int32
            Console.WriteLine("Before removal - Areas count: " + fcc.Count);
            fcc.RemoveArea(0, 0, 1, 1); // Remove the initial area
            Console.WriteLine("After removal - Areas count: " + fcc.Count);
            
            // إضافة منطقة جديدة
            CellArea newArea = CellArea.CreateCellArea(1, 1, 1, 1);
            fcc.AddArea(newArea);
            Console.WriteLine("After adding new area - Areas count: " + fcc.Count);
        }
    }
}
```

### انظر أيضًا

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


