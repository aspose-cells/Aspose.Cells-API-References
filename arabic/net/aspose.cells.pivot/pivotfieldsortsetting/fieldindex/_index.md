---
title: "PivotFieldSortSetting.FieldIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFieldSortSetting. تمثل فهرس الحقل الذي يتم فرزه. 1 يعني فرز PivotField حسب التسميات، أما غير ذلك فيعني الفرز حسب حقل البيانات"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldsortsetting/fieldindex/
---
## PivotFieldSortSetting.FieldIndex property

تمثل فهرس الحقل الذي يتم فرزه. -1 يعني فرز PivotField حسب التسميات، أما غير ذلك فيعني الفرز حسب حقل البيانات.

```csharp
[Obsolete("Use PivotFieldSortSetting.SortBy property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int FieldIndex { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotFieldSortSetting.SortBy. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // احصل على إعداد فرز حقل المحور
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;

            // عرض قيمة FieldIndex الحالية
            Console.WriteLine("Current FieldIndex value: " + sortSetting.FieldIndex);

            // ملاحظة: FieldIndex للقراءة فقط ولا يمكن إنشاء PivotFieldSortSetting مباشرة
            // لأنه لا يحتوي على مُنشئ عام. يمكننا فقط العمل مع النسخة الحالية
            // تم الحصول عليها من خاصية SortSetting لحقل المحور.

            // تحديث جدول المحور لتطبيق التغييرات
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // حفظ النتيجة
            workbook.Save("PivotFieldSortSettingFieldIndexDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


