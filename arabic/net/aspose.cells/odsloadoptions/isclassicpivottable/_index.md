---
title: "OdsLoadOptions.IsClassicPivotTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsLoadOptions. تشير إلى ما إذا كان جدول المحور كلاسيكيًا"
type: docs
url: /ar/net/aspose.cells/odsloadoptions/isclassicpivottable/
---
## OdsLoadOptions.IsClassicPivotTable property

يشير إلى ما إذا كان جدول المحور كلاسيكيًا.

```csharp
public bool IsClassicPivotTable { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsLoadOptionsPropertyIsClassicPivotTableDemo
    {
        public static void Run()
        {
            // أنشئ ملف ODS تجريبي مع جدول محوري
            CreateSampleOdsWithPivotTable();

            // حمّل مع تعيين IsClassicPivotTable إلى true
            OdsLoadOptions loadOptionsTrue = new OdsLoadOptions();
            loadOptionsTrue.IsClassicPivotTable = true;
            
            Workbook workbookTrue = new Workbook("SamplePivot.ods", loadOptionsTrue);
            Console.WriteLine("Loaded with IsClassicPivotTable = true");
            Console.WriteLine("PivotTable fields count: " + workbookTrue.Worksheets[0].PivotTables[0].BaseFields.Count);

            // حمّل مع تعيين IsClassicPivotTable إلى false
            OdsLoadOptions loadOptionsFalse = new OdsLoadOptions();
            loadOptionsFalse.IsClassicPivotTable = false;
            
            Workbook workbookFalse = new Workbook("SamplePivot.ods", loadOptionsFalse);
            Console.WriteLine("\nLoaded with IsClassicPivotTable = false");
            Console.WriteLine("PivotTable fields count: " + workbookFalse.Worksheets[0].PivotTables[0].BaseFields.Count);
        }

        private static void CreateSampleOdsWithPivotTable()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ملء بيانات عينة
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Electronics";
            cells["A3"].Value = "Clothing";
            cells["A4"].Value = "Books";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1500;
            cells["B3"].Value = 800;
            cells["B4"].Value = 200;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesReport");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // أضف حقل صف (Category)
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // أضف حقل بيانات (Sales) وحدد اسم العرض
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.DataFields[dataFieldIndex].DisplayName = "Total Sales";

            // احفظ كملف ODS
            workbook.Save("SamplePivot.ods", SaveFormat.Ods);
        }
    }
}
```

### انظر أيضًا

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


