---
title: "ChartCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartCollection. تضيف مخططًا إلى المجموعة"
type: docs
url: /ar/net/aspose.cells.charts/chartcollection/add/
---
## Add(ChartType, int, int, int, int) {#add}

يضيف مخططًا إلى المجموعة.

```csharp
public int Add(ChartType type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ChartType | نوع المخطط |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| الصف السفلي | Int32 | فهرس الصف السفلي الأيمن |
| rightColumn | Int32 | فهرس العمود السفلي الأيمن |

### قيمة الإرجاع

[`Chart`](../../chart/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 1; i <= 10; i++)
            {
                sheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                sheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // إضافة مخطط باستخدام المعلمات المحددة
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("=Sheet1!$A$1:$B$11", true);

            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, int, int, int, int) {#add_2}

يضيف مخططًا إلى المجموعة.

```csharp
[Obsolete("Use ChartCollection.Add(ChartType, string, bool ,int , int, int, int ) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ChartType type, string dataRange, int topRow, int leftColumn, int rightRow, 
    int bottomColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ChartType | نوع المخطط |
| dataRange | String | يحدد نطاق البيانات للمخطط |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| rightRow | Int32 | فهرس الصف السفلي الأيمن |
| bottomColumn | Int32 | فهرس العمود السفلي الأيمن |

### قيمة الإرجاع

[`Chart`](../../chart/) object index.

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية `Add`. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithChartTypeStringInt32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // استدعاء طريقة Add مع المعلمات (ChartType, String, Int32, Int32, Int32, Int32)
                int chartIndex = worksheet.Charts.Add(
                    ChartType.Column,          // Chart type
                    "A1:B4",                  // Data range
                    0,                        // Top row position
                    3,                        // Left column position
                    15,                       // Bottom row position
                    8                         // Right column position
                );

                Console.WriteLine("Chart added successfully at index: " + chartIndex);
                
                // الوصول إلى المخطط الذي تم إنشاؤه حديثًا
                Chart chart = worksheet.Charts[chartIndex];
                chart.Title.Text = "Sample Column Chart";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("ChartCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(byte[], string, bool, int, int, int, int) {#add_3}

يضيف مخططًا باستخدام قالب مسبق.

```csharp
public int Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| بيانات | Byte[] | بيانات ملف قالب المخطط (.crtx). |
| dataRange | String | يحدد نطاق البيانات للمخطط |
| isVertical | منطقي | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| rightRow | Int32 | فهرس الصف السفلي الأيمن |
| bottomColumn | Int32 | فهرس العمود السفلي الأيمن |

### قيمة الإرجاع

[`Chart`](../../chart/) object index.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithByteArrayStringBooleanInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إنشاء مصفوفة بايت تمثل بيانات المخطط (مثال مبسط)
            byte[] chartData = new byte[] { 0x01, 0x02, 0x03 };

            try
            {
                // استدعِ طريقة Add مع معلمات محددة
                int chartIndex = worksheet.Charts.Add(
                    chartData,          // Byte[] data
                    "A1:B4",            // String dataRange
                    true,               // Boolean isVertical
                    0,                  // Int32 topRow
                    0,                  // Int32 leftColumn
                    15,                 // Int32 rightRow
                    8                   // Int32 bottomColumn
                );

                Console.WriteLine($"Chart added successfully at index: {chartIndex}");

                // الوصول إلى المخطط المضاف
                Chart chart = worksheet.Charts[chartIndex];
                chart.Type = ChartType.Column;

                // حفظ النتيجة
                workbook.Save("ChartCollectionMethodAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, bool, int, int, int, int) {#add_1}

يضيف مخططًا إلى المجموعة.

```csharp
public int Add(ChartType type, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ChartType | نوع المخطط |
| dataRange | String | يحدد نطاق البيانات للمخطط |
| isVertical | منطقي | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| rightRow | Int32 | فهرس الصف السفلي الأيمن |
| bottomColumn | Int32 | فهرس العمود السفلي الأيمن |

### قيمة الإرجاع

[`Chart`](../../chart/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeStringBooleanInt32IntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);

            // إضافة مخطط بالمعلمات المحددة
            int chartIndex = worksheet.Charts.Add(ChartType.Column, "A1:C3", true, 4, 4, 14, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


