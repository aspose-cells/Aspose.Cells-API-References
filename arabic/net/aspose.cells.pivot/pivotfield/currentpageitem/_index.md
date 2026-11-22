---
title: "PivotField.CurrentPageItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. يحصل أو يضبط العنصر الصفحي المعروض حاليًا لهذا الحقل المحوري للصفحة فقط"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/currentpageitem/
---
## PivotField.CurrentPageItem property

يحصل أو يعيّن عنصر الصفحة المعروض حاليًا لهذا الحقل المحوري (حقل الصفحة فقط).

```csharp
public short CurrentPageItem { get; set; }
```

### ملاحظات

استخدم [`AllPageItemsIndex`](../../pivotitem/allpageitemsindex/) (0x7FFD) كقيمة إشارة للدلالة على "Select All". هذا علامة معرفة مسبقًا وليس فهرس عنصر صالح.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyCurrentPageItemDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Apple";
            worksheet.Cells["A5"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["B5"].Value = "East";
            
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 1500;
            worksheet.Cells["C5"].Value = 3000;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقول
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Product");
            
            // تحديث البيانات
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احصل على حقول الصفحة
            PivotFieldCollection pageFields = pivotTable.PageFields;
            
            // عرض العناصر الصفحية الحالية
            Console.WriteLine("Initial CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // تغيير العنصر الصفحي الحالي
            pageFields[0].CurrentPageItem = 1; // Change to Banana
            Console.WriteLine("After Change CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // احفظ المصنف
            workbook.Save("PivotFieldCurrentPageItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


