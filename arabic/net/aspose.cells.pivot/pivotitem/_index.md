---
title: "الفئة PivotItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Pivot.PivotItem. يمثل عنصرًا في تقرير PivotField."
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/
---
## PivotItem class

يمثل عنصرًا في تقرير PivotField.

```csharp
public class PivotItem
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Index](../../aspose.cells.pivot/pivotitem/index/) { get; set; } | (**Obsolete.**) يحصل على فهرس العنصر المحوري في حقل الذاكرة المؤقتة. |
| [IsCalculatedItem](../../aspose.cells.pivot/pivotitem/iscalculateditem/) { get; } | يشير إلى ما إذا كان هذا العنصر المحوري عنصر صيغة محسوبة. |
| [IsDetailHidden](../../aspose.cells.pivot/pivotitem/isdetailhidden/) { get; set; } | يحصل ويضبط ما إذا كان تفصيل هذا العنصر المحوري مخفيًا. |
| [IsFormula](../../aspose.cells.pivot/pivotitem/isformula/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان هذا العنصر المحوري عنصر صيغة محسوبة. |
| [IsHidden](../../aspose.cells.pivot/pivotitem/ishidden/) { get; set; } | يحصل ويضبط ما إذا كان العنصر المحوري مخفيًا. |
| [IsHideDetail](../../aspose.cells.pivot/pivotitem/ishidedetail/) { get; set; } | (**Obsolete.**) يحصل ويضبط ما إذا كان العنصر المحوري يخفي التفاصيل. |
| [IsMissing](../../aspose.cells.pivot/pivotitem/ismissing/) { get; } | يشير إلى ما إذا تم إزالة العنصر من مصدر البيانات. |
| [Name](../../aspose.cells.pivot/pivotitem/name/) { get; set; } | يحصل على اسم العنصر المحوري. |
| [Position](../../aspose.cells.pivot/pivotitem/position/) { get; set; } | تحديد فهرس هذا العنصر في جميع PivotItems الخاصة بالحقل. |
| [PositionInSameParentNode](../../aspose.cells.pivot/pivotitem/positioninsameparentnode/) { get; set; } | (**Obsolete.**) تحديد فهرس الموضع في PivotItems تحت نفس العقدة الأصلية. |
| [Value](../../aspose.cells.pivot/pivotitem/value/) { get; } | يحصل على قيمة العنصر المحوري |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetDateTimeValue](../../aspose.cells.pivot/pivotitem/getdatetimevalue/)() | يحصل على قيمة التاريخ والوقت للعنصر المحوري. إذا كانت القيمة فارغة، سيعيد DateTime.MinValue |
| [GetDoubleValue](../../aspose.cells.pivot/pivotitem/getdoublevalue/)() | يحصل على القيمة المزدوجة لعنصر المحور. إذا كانت القيمة فارغة أو ليست رقمًا، سيعيد 0 |
| [GetFormula](../../aspose.cells.pivot/pivotitem/getformula/)() | يحصل على صيغة هذا العنصر المحسوب. يعمل فقط عندما يكون هذا العنصر عنصرًا محسوبًا. |
| [GetStringValue](../../aspose.cells.pivot/pivotitem/getstringvalue/)() | يحصل على القيمة النصية لعنصر المحور. إذا كانت القيمة فارغة، سيعيد "" |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move)(int) | ينقل العنصر للأعلى أو للأسفل في حقل المحور |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move_1)(int, bool) | (**Obsolete.**) ينقل العنصر للأعلى أو للأسفل |

## الحقول

| الاسم | الوصف |
| --- | --- |
| const [AllPageItemsIndex](../../aspose.cells.pivot/pivotitem/allpageitemsindex/) | فهرس الحارس لتحديد-الكل لعناصر الصفحة (0x7FFD، ليس فهرسًا صالحًا) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemDemo
    {
        public static void PivotItemExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // أضف جدولًا محوريًا إلى ورقة العمل
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // الوصول إلى عناصر المحور
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            int pivotItemCount = pivotItems.Count;
            Console.WriteLine("Number of Pivot Items: " + pivotItemCount);
            for(int i = 0; i < pivotItemCount; i++)
            {
                PivotItem pivotItem = pivotItems[i];
                // اطبع اسم العنصر المحوري
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);

                // تعيين الخصائص
                pivotItem.IsHidden = false;
                pivotItem.Position = 1;
                pivotItem.IsHideDetail = false;

                // اطبع قيمة العنصر المحوري
                Console.WriteLine("Pivot Item Value: " + pivotItem.Value);

                // استخدم الطرق
                string stringValue = pivotItem.GetStringValue();
                double doubleValue = pivotItem.GetDoubleValue();
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();

                Console.WriteLine("String Value: " + stringValue);
                Console.WriteLine("Double Value: " + doubleValue);
                Console.WriteLine("DateTime Value: " + dateTimeValue);
            }

            // احفظ المصنف
            workbook.Save("PivotItemExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


