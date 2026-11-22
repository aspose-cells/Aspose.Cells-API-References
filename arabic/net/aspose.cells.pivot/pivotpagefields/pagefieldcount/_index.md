---
title: "PivotPageFields.PageFieldCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotPageFields. تحصل على عدد حقول الصفحة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotpagefields/pagefieldcount/
---
## PivotPageFields.PageFieldCount property

يحصل على عدد حقول الصفحة.

```csharp
public int PageFieldCount { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsPropertyPageFieldCountDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // أنشئ أوراق عمل نموذجية مع البيانات
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Data1";
            FillSampleData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Data2");
            FillSampleData(sheet2);

            // أنشئ ورقة محورية
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");

            // أنشئ مثيل PivotPageFields
            PivotPageFields pageFields = new PivotPageFields();

            // أضف حقول الصفحة لتوضيح خاصية PageFieldCount
            pageFields.AddPageField(new string[] { "Category1", "Category2" });
            pageFields.AddPageField(new string[] { "Region1", "Region2" });

            try
            {
                // اعرض قيمة خاصية PageFieldCount
                Console.WriteLine("Number of page fields: " + pageFields.PageFieldCount);

                // إضافة تعريف لحقول الصفحة
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                pageFields.AddIdentify(1, new int[] { 1, 0 });

                // تحقق من بقاء العدد كما هو بعد إضافة التعريفات
                Console.WriteLine("PageFieldCount after adding identifications: " + pageFields.PageFieldCount);

                // إنشاء جدول محوري باستخدام حقول الصفحة
                string[] sources = { "=Data1!A1:C4", "=Data2!A1:C4" };
                pivotSheet.PivotTables.Add(sources, false, pageFields, "E3", "DemoPivot");

                // احفظ المصنف
                workbook.Save("PageFieldCountDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static void FillSampleData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Value");

            cells["A2"].PutValue("Category1");
            cells["B2"].PutValue("Region1");
            cells["C2"].PutValue(100);

            cells["A3"].PutValue("Category2");
            cells["B3"].PutValue("Region2");
            cells["C3"].PutValue(200);
        }
    }
}
```

### انظر أيضًا

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


