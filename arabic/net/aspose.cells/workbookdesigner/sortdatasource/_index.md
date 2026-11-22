---
title: "WorkbookDesigner.SortDataSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookDesigner. تشير إلى ما إذا كان مصدر البيانات يتم فرزه"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/sortdatasource/
---
## WorkbookDesigner.SortDataSource property

يشير إلى ما إذا كان يتم فرز مصدر البيانات.

```csharp
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SortDataSource { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته. سيتم فرز مصدر بيانات Json إذا احتوت العلامة الذكية على معلمات تصاعدية وتنازلية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerPropertySortDataSourceDemo
    {
        public static void Run()
        {
            // إنشاء DataTable عينة ببيانات غير مرتبة
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID", typeof(int));
            dataTable.Columns.Add("ProductName", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // إضافة بيانات عينة بترتيب غير مرتب
            dataTable.Rows.Add(3, "Product C", 15.99m);
            dataTable.Rows.Add(1, "Product A", 10.50m);
            dataTable.Rows.Add(2, "Product B", 12.75m);

            // إنشاء مصنف باستخدام العلامات الذكية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إعداد العلامات الذكية في ورقة العمل
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$Price");

            try
            {
                // إنشاء مثيل WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // عرض قيمة SortDataSource الأولية
                Console.WriteLine($"Initial SortDataSource value: {designer.SortDataSource}");

                // تعيين مصدر البيانات بدون فرز
                designer.SortDataSource = false;
                designer.SetDataSource(dataTable);
                designer.Process();

                // حفظ النتيجة غير المرتبة
                workbook.Save("UnsortedOutput.xlsx");
                Console.WriteLine("Unsorted data saved to UnsortedOutput.xlsx");

                // إنشاء مصنف جديد لعرض الترتيب
                Workbook sortedWorkbook = new Workbook();
                Worksheet sortedSheet = sortedWorkbook.Worksheets[0];
                sortedSheet.Cells["A1"].PutValue("&=$ProductID");
                sortedSheet.Cells["B1"].PutValue("&=$ProductName");
                sortedSheet.Cells["C1"].PutValue("&=$Price");

                // إنشاء مصمم جديد مع تمكين الفرز
                WorkbookDesigner sortedDesigner = new WorkbookDesigner(sortedWorkbook);
                sortedDesigner.SortDataSource = true;
                sortedDesigner.SetDataSource(dataTable);
                sortedDesigner.Process();

                // حفظ النتيجة المرتبة
                sortedWorkbook.Save("SortedOutput.xlsx");
                Console.WriteLine("Sorted data saved to SortedOutput.xlsx");
                Console.WriteLine($"Final SortDataSource value: {sortedDesigner.SortDataSource}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


