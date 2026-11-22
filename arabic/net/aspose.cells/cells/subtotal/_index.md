---
title: "Cells.Subtotal"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تنشئ مجاميع فرعية للنطاق"
type: docs
url: /ar/net/aspose.cells/cells/subtotal/
---
## Subtotal(CellArea, int, ConsolidationFunction, int[]) {#subtotal}

ينشئ المجاميع الفرعية للنطاق.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | CellArea | النطاق |
| groupBy | Int32 | الحقل لتجميعه، كإزاحة عددية تبدأ من الصفر |
| دالة | ConsolidationFunction | دالة التجميع الفرعي. |
| totalList | Int32[] | مصفوفة من إزاحات الحقول ذات القاعدة الصفرية، تشير إلى الحقول التي تُضاف إليها المجاميع الفرعية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات عينة للتجميع الفرعي
            CreateSampleData(worksheet);

            // تحديد نطاق الخلايا الذي يحتوي على البيانات (A1:C6)
            CellArea cellArea = CellArea.CreateCellArea(0, 0, 5, 2);

            try
            {
                // استدعاء طريقة Subtotal مع المعلمات:
                // - التجميع حسب العمود 0 (المنطقة)
                // - استخدام دالة SUM
                // - تطبيق على العمود 2 (المبيعات)
                worksheet.Cells.Subtotal(
                    cellArea,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 }
                );

                Console.WriteLine("Subtotal added successfully for parameters (CellArea, 0, Sum, [2])");
                
                // تمت إزالة أساليب ExpandColumnLevel و ExpandRowLevel لإصلاح أخطاء التجميع
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Subtotal method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // إنشاء صف الرأس
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");

            // إنشاء صفوف البيانات
            object[,] data = new object[,] {
                {"North", "Widget", 5000},
                {"North", "Gadget", 3000},
                {"South", "Widget", 6000},
                {"South", "Gadget", 4000},
                {"West", "Widget", 4500}
            };

            // ملء البيانات بدءًا من الصف 2 (فهرس يبدأ من الصفر 1)
            for (int i = 0; i < data.GetLength(0); i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(data[i, 0]);
                worksheet.Cells[i + 1, 1].PutValue(data[i, 1]);
                worksheet.Cells[i + 1, 2].PutValue(data[i, 2]);
            }
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Subtotal(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) {#subtotal_1}

ينشئ المجاميع الفرعية للنطاق.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList, 
    bool replace, bool pageBreaks, bool summaryBelowData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | CellArea | النطاق |
| groupBy | Int32 | الحقل لتجميعه، كإزاحة عددية تبدأ من الصفر |
| دالة | ConsolidationFunction | دالة التجميع الفرعي. |
| totalList | Int32[] | مصفوفة من إزاحات الحقول ذات القاعدة الصفرية، تشير إلى الحقول التي تُضاف إليها المجاميع الفرعية. |
| استبدال | منطقي | يشير إلى ما إذا كان سيستبدل المجاميع الفرعية الحالية |
| فواصل الصفحات | منطقي | يشير إلى ما إذا كان سيضيف فاصل صفحة بين المجموعات |
| ملخص تحت البيانات | منطقي | يشير إلى ما إذا كان يتم إضافة ملخص أسفل البيانات. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء بيانات عينة للتجميع الفرعي
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            object[,] data = new object[,] {
                { "Fruits", "Apple", 1500 },
                { "Fruits", "Orange", 2500 },
                { "Vegetables", "Carrot", 1800 },
                { "Vegetables", "Potato", 3000 },
                { "Fruits", "Banana", 2000 }
            };

            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row + 1, col].PutValue(data[row, col]);
                }
            }

            try
            {
                // تحديد نطاق الخلايا للتجميع الفرعي (A1:C6)
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 5;
                area.EndColumn = 2;

                // استدعاء Subtotal مع المعلمات:
                // - التجميع حسب العمود الأول (فهرس يبدأ من الصفر 0)
                // - استخدام دالة Sum
                // - تطبيق على العمود الثالث (فهرس يبدأ من الصفر 2)
                // - استبدال المجاميع الفرعية الموجودة، فواصل الصفحات بين المجموعات، ملخص تحت البيانات
                cells.Subtotal(
                    area,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 },
                    true,
                    true,
                    true
                );

                Console.WriteLine("Subtotal added successfully for parameters: (CellArea, Int32, ConsolidationFunction, Int32[], Boolean, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating subtotal: {ex.Message}");
            }

            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


