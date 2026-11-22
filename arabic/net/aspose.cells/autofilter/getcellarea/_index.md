---
title: "AutoFilter.GetCellArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. تحصل على CellArea حيث يطبق هذا AutoFilter"
type: docs
url: /ar/net/aspose.cells/autofilter/getcellarea/
---
## GetCellArea() {#getcellarea}

يحصل على [`CellArea`](../../cellarea/) حيث يُطبق هذا AutoFilter.

```csharp
public CellArea GetCellArea()
```

### قيمة الإرجاع

المساحة التي يُطبق عليها هذا الفلتر

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ملء بيانات عينة لتوضيح AutoFilter
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Category");
            cells["C1"].PutValue("Price");

            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue("Fruit");
            cells["C2"].PutValue(2.5);

            cells["A3"].PutValue("Carrot");
            cells["B3"].PutValue("Vegetable");
            cells["C3"].PutValue(1.2);

            cells["A4"].PutValue("Banana");
            cells["B4"].PutValue("Fruit");
            cells["C4"].PutValue(3.1);

            // تطبيق AutoFilter على رؤوس الأعمدة (فهرس الصف 0) التي تغطي الأعمدة A-C (0-2)
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 2);

            try
            {
                // احصل على CellArea حيث تم تطبيق AutoFilter
                CellArea result = autoFilter.GetCellArea();

                // إخراج إحداثيات نطاق AutoFilter
                Console.WriteLine("AutoFilter applied to cell area:");
                Console.WriteLine($"Start Row: {result.StartRow}");
                Console.WriteLine($"Start Column: {result.StartColumn}");
                Console.WriteLine($"End Row: {result.EndRow}");
                Console.WriteLine($"End Column: {result.EndColumn}");

                // تطبيق مرشح بسيط لتوضيح الوظيفة (اختياري)
                autoFilter.Filter(1, "Fruit"); // Filter "Category" column (index 1) for "Fruit"
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea method: {ex.Message}");
            }

            // حفظ المصنف مع AutoFilter المطبق
            workbook.Save("AutoFilterMethodGetCellAreaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellArea(bool) {#getcellarea_1}

يحصل على [`CellArea`](../../cellarea/) حيث يُطبق AutoFilter المحدد.

```csharp
public CellArea GetCellArea(bool refreshAppliedRange)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| refreshAppliedRange | منطقي | ما إذا كان يجب تحديث النطاق المطبق. بالنسبة للنطاق المطبق ل AutoFilter، قد يتغير الصف الأخير عندما تتغير بيانات الخلايا. إذا كانت هذه العلامة true، فسيتم إعادة حساب الصف الأخير من النطاق وفقًا لبيانات الخلايا الحالية. |

### قيمة الإرجاع

المساحة التي يُطبق عليها هذا الفلتر

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير بيانات عينة لـ AutoFilter
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");

            // تعيين نطاق AutoFilter (الصف 0 إلى 3، العمود 0)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // استدعاء GetCellArea مع refreshAppliedRange=true
                CellArea result = worksheet.AutoFilter.GetCellArea(true);

                // عرض النطاق المطبق لـ AutoFilter
                Console.WriteLine($"AutoFilter Range: StartRow={result.StartRow}, " +
                    $"StartColumn={result.StartColumn}, EndRow={result.EndRow}, " +
                    $"EndColumn={result.EndColumn}");

                Console.WriteLine("GetCellArea method executed successfully with boolean parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("AutoFilterMethodGetCellAreaWithBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


