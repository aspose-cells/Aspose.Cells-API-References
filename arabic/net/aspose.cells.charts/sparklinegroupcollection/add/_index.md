---
title: "SparklineGroupCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SparklineGroupCollection. تضيف SparklineGroup مع Sparkline إلى المجموعة"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroupcollection/add/
---
## Add(SparklineType) {#add}

تضيف [`SparklineGroup`](../../sparklinegroup/) مع [`Sparkline`](../../sparkline/) إلى المجموعة.

```csharp
public int Add(SparklineType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | SparklineType | يحدد نوع مجموعة Sparkline. |

### قيمة الإرجاع

[`SparklineGroup`](../../sparklinegroup/) object index.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodAddWithSparklineTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للمخططات الصغيرة
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["A5"].PutValue(9);

            try
            {
                // احصل على مجموعة مجموعات Sparkline
                SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;

                // استدعِ طريقة Add مع معامل SparklineType
                int index = sparklineGroups.Add(SparklineType.Line);

                // تكوين مجموعة Sparkline
                SparklineGroup group = sparklineGroups[index];
                group.Sparklines.Add("A1:A5", 5, 0);

                Console.WriteLine("Sparkline group added successfully with type: Line");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("SparklineGroupCollectionMethodAddWithSparklineTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(SparklineType, string, bool, CellArea) {#add_1}

تضيف [`SparklineGroup`](../../sparklinegroup/) مع بعض [`Sparkline`](../../sparkline/) إلى المجموعة.

```csharp
public int Add(SparklineType type, string dataRange, bool isVertical, CellArea locationRange)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | SparklineType | يحدد نوع مجموعة Sparkline. |
| dataRange | String | يحدد نطاق البيانات لمجموعة Sparkline. |
| isVertical | منطقي | يحدد ما إذا كان سيتم رسم sparklines من نطاق البيانات حسب الصف أو حسب العمود. |
| locationRange | CellArea | يحدد مكان وضع المخططات الصغيرة. |

### قيمة الإرجاع

[`SparklineGroup`](../../sparklinegroup/) object index.

### ملاحظات

هذه الطريقة ستنشئ sparklines أيضًا. إذا كان *isVertical* صحيحًا، يجب أن يكون عدد الصفوف في dataRange و locationRange متساويًا. إذا كان *isVertical* خاطئًا، يجب أن يكون عدد الأعمدة في dataRange و locationRange متساويًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionMethodAddWithSparklineTypeStringBooleanCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة للمخططات الصغيرة
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(3);
            sheet.Cells["C1"].PutValue(8);
            
            // أضف مجموعة Sparkline مع المعلمات المحددة
            sheet.SparklineGroups.Add(
                SparklineType.Line, 
                "A1:C1", 
                false, 
                CellArea.CreateCellArea("D1", "D1")
            );
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SparklineType](../../sparklinetype/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


