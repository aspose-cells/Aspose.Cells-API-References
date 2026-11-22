---
title: "CellsHelper.CellNameToIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. يحصل على فهارس الصف والعمود للخلية وفقًا لاسمها"
type: docs
url: /ar/net/aspose.cells/cellshelper/cellnametoindex/
---
## CellsHelper.CellNameToIndex method

يحصل على مؤشرات الصف والعمود للخلية وفقًا لاسمها.

```csharp
public static void CellNameToIndex(string cellName, out int row, out int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية. |
| صف | Int32& | فهرس صف الإخراج |
| عمود | Int32& | فهرس عمود الإخراج |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodCellNameToIndexWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // تهيئة المتغيرات لتخزين فهارس الصف والعمود
            int rowIndex = -1;
            int columnIndex = -1;
            string cellName = "C5";

            try
            {
                // استدعِ طريقة CellNameToIndex لتحويل اسم الخلية إلى مؤشرات الصف والعمود
                CellsHelper.CellNameToIndex(cellName, out rowIndex, out columnIndex);

                // عرض النتائج
                Console.WriteLine($"Cell name: {cellName}");
                Console.WriteLine($"Row index: {rowIndex}");
                Console.WriteLine($"Column index: {columnIndex}");

                // أنشئ دفتر عمل وبيّن استخدام المؤشرات
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // الوصول إلى الخلية باستخدام المؤشرات المستخرجة
                Cell cell = worksheet.Cells[rowIndex, columnIndex];
                cell.PutValue("Test Value");

                // احفظ المصنف
                workbook.Save("CellNameToIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CellNameToIndex method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


