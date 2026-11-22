---
title: "PivotTable.Move"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تنقل PivotTable إلى موقع مختلف في ورقة العمل"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/move/
---
## Move(int, int) {#move}

ينقل جدول المحور إلى موقع مختلف في ورقة العمل.

```csharp
[Obsolete("Use PivotTable.MoveTo() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### ملاحظات

ملاحظة: هذه الخاصية الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.MoveTo(). ستُزال هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // احسب البيانات لملء جدول المحور
            pivotTable.CalculateData();

            Console.WriteLine("Pivot table created at E3");

            try
            {
                // نقل جدول البيفوت إلى موقع جديد (الصف 10، العمود 5)
                pivotTable.Move(10, 5);
                Console.WriteLine("Pivot table moved to row 10, column 5");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("PivotTableMethodMoveWithInt32Int32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(string) {#move_1}

ينقل جدول المحور إلى موقع مختلف في ورقة العمل.

```csharp
[Obsolete("Use PivotTable.MoveTo() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(string destCellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destCellName | String | اسم الخلية الوجهة. |

### ملاحظات

ملاحظة: هذه الخاصية الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.MoveTo(). ستُزال هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // نقل جدول البيفوت إلى موقع جديد باستخدام اسم الخلية
                pivotTable.Move("G10");

                Console.WriteLine("PivotTable moved successfully to G10");
                Console.WriteLine($"New location: {pivotTable.TableRange1.StartRow}, {pivotTable.TableRange1.StartColumn}");

                // احفظ المصنف
                workbook.Save("PivotTableMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error moving PivotTable: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


