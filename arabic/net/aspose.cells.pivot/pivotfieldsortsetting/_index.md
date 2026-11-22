---
title: "فئة PivotFieldSortSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Pivot.PivotFieldSortSetting class. يمثل الإعداد لفرز حقول المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldsortsetting/
---
## PivotFieldSortSetting class

يمثل الإعداد لفرز الحقول المحورية.

```csharp
public class PivotFieldSortSetting
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Cell](../../aspose.cells.pivot/pivotfieldsortsetting/cell/) { get; } | يتم الفرز حسب القيم في أي صف أو عمود. |
| [FieldIndex](../../aspose.cells.pivot/pivotfieldsortsetting/fieldindex/) { get; set; } | (**Obsolete.**) يمثل فهرس الحقل الذي يتم فرزه حسبه. -1 يعني فرز PivotField حسب التسميات، والآخرون يعني فرز حسب حقل البيانات. |
| [IsSimpleSort](../../aspose.cells.pivot/pivotfieldsortsetting/issimplesort/) { get; set; } | يشير إلى ما إذا كان سيتم تطبيق عملية فرز بيانات بسيطة. |
| [IsSortByLabels](../../aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/) { get; } | يشير إلى ما إذا كان سيتم فرز الحقل بنفسه أو حقل البيانات. |
| [LineTypeSortedBy](../../aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/) { get; } | نوع سطر المحور المرتب حسب. |
| [SortBy](../../aspose.cells.pivot/pivotfieldsortsetting/sortby/) { get; set; } | يمثل فهرس الحقل المرتب حسب. قيمة -1 تشير إلى الفرز حسب قيم العنصر المحوري نفسه. عندما يكون أكبر من أو يساوي الصفر، يمثل فهرس حقل البيانات في منطقة البيانات. |
| [SortType](../../aspose.cells.pivot/pivotfieldsortsetting/sorttype/) { get; set; } | يمثل [`SortOrder`](../../aspose.cells/sortorder/). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotFieldSortSettingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["B4"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // احصل على إعداد فرز حقل المحور من جدول المحور
            // ملاحظة: هذا يفترض أن جدول المحور يحتوي على إعدادات فرز يمكننا الوصول إليها
            // نظرًا لأنه لا يمكننا إنشاء PivotFieldSortSetting جديد مباشرة
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;
            
            // عرض الخصائص (للقراءة فقط)
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("IsSortByLabels: " + sortSetting.IsSortByLabels);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("LineTypeSortedBy: " + sortSetting.LineTypeSortedBy);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);
            Console.WriteLine("Cell: " + sortSetting.Cell);

            // تطبيق الفرز على جدول المحور (سيتم تنفيذ الفرز الفعلي من خلال طرق جدول المحور)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // حفظ النتيجة
            workbook.Save("PivotFieldSortSettingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


