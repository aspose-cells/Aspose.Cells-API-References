---
title: "الفئة PivotShowValuesSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Pivot.PivotShowValuesSetting. تمثل الإعدادات المتعلقة بعرض القيم عندما يكون حساب ShowDataAs قيد الاستخدام"
type: docs
url: /ar/net/aspose.cells.pivot/pivotshowvaluessetting/
---
## PivotShowValuesSetting class

يمثل الإعدادات المتعلقة بعرض القيم عندما يكون حساب ShowDataAs قيد الاستخدام.

```csharp
public class PivotShowValuesSetting
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/) { get; set; } | تمثل الحقل الأساسي لحساب ShowDataAs عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [BaseFieldName](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldname/) { get; } | يحصل على تسمية حقل الأساس للـ Pivot. |
| [BaseItemCaption](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemcaption/) { get; } | يحصل على تسمية عنصر الـ Pivot في الحقل الأساسي. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/) { get; set; } | تمثل الفهرس المخصص لعنصر الـ Pivot في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [BaseItemPositionType](../../aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/) { get; set; } | (**Obsolete.**) تمثل نوع عنصر الـ Pivot الأساسي في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام. لأن PivotItemPosition.Custom للقراءة فقط، إذا كنت بحاجة إلى تعيين PivotItemPosition.Custom، يرجى تعيين الخاصية PivotField.BaseItemIndex. |
| [CalculationType](../../aspose.cells.pivot/pivotshowvaluessetting/calculationtype/) { get; set; } | (**Obsolete.**) تمثل طريقة عرض قيم حقل البيانات في تقرير الـ Pivot. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotshowvaluessetting/showvaluesas/) { get; set; } | يحصل ويضبط طريقة عرض قيم حقل البيانات في تقرير الـ Pivot. |

## الحقول

| الاسم | الوصف |
| --- | --- |
| const [NextPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/nextpivotitem/) | فهرس العنصر الأساسي الخاص: استخدم عنصر الـ Pivot التالي. صالح لحسابات "Show Values As"؛ فعال في Excel 2010 وما بعده. |
| const [PreviousPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/previouspivotitem/) | فهرس العنصر الأساسي الخاص: استخدم عنصر الـ Pivot السابق. صالح لحسابات "Show Values As"؛ فعال في Excel 2010 وما بعده. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingDemo
    {
        public static void PivotShowValuesSettingExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            // أضف جدولًا محوريًا إلى ورقة العمل
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // الوصول إلى حقل البيانات
            PivotField dataField = pivotTable.DataFields[0];

            // الوصول إلى خاصية ShowValuesSetting
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            // تعيين خصائص PivotShowValuesSetting
            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0; // Base field index
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1; // Base item index

            // تحديث وحساب بيانات جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotShowValuesSettingExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


