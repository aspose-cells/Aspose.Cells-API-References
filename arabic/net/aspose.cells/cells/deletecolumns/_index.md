---
title: "Cells.DeleteColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحذف عدة أعمدة"
type: docs
url: /ar/net/aspose.cells/cells/deletecolumns/
---
## DeleteColumns(int, int, bool) {#deletecolumns_1}

يحذف عدة أعمدة.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, bool updateReference)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود الأول الذي سيتم حذفه. |
| totalColumns | Int32 | عدد الأعمدة التي سيتم حذفها. |
| updateReference | منطقي | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // إضافة صيغة تشير إلى هذه الأعمدة
            worksheet.Cells["D1"].Formula = "=SUM(A2:C2)";

            Console.WriteLine("Before deleting columns:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1: " + worksheet.Cells["C1"].Value);
            Console.WriteLine("D1 formula: " + worksheet.Cells["D1"].Formula);

            // حذف العمود B (فهرس 1) وتحريك الأعمدة المتبقية إلى اليسار
            worksheet.Cells.DeleteColumns(1, 1, true);

            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1 formula: " + worksheet.Cells["C1"].Formula);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumns(int, int, DeleteOptions) {#deletecolumns}

يحذف عدة أعمدة.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود الأول الذي سيتم حذفه. |
| totalColumns | Int32 | عدد الأعمدة التي سيتم حذفها. |
| خيارات | DeleteOptions | خيارات عملية الحذف |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodDeleteColumnsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بيانات نموذجية في الأعمدة A‑E
            for (int col = 0; col < 5; col++)
            {
                worksheet.Cells[0, col].Value = $"Column {(char)('A' + col)}";
                worksheet.Cells[1, col].Value = $"Data{col + 1}";
            }

            // إنشاء DeleteOptions وتكوين الإعدادات
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Update references in other cells
            };

            try
            {
                // حذف عمودين بدءًا من العمود B (فهرس 1)
                worksheet.Cells.DeleteColumns(1, 2, options);
                
                Console.WriteLine("Deleted columns B and C successfully");
                
                // عرض البيانات المتبقية في العمود B (العمود D الأصلي)
                Console.WriteLine($"New column B value: {worksheet.Cells[1, 1].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteColumns: {ex.Message}");
            }
            
            // احفظ المصنف المعدل
            workbook.Save("DeleteColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


