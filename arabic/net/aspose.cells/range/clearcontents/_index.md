---
title: "Range.ClearContents"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تُمسح محتويات هذا النطاق"
type: docs
url: /ar/net/aspose.cells/range/clearcontents/
---
## Range.ClearContents method

يمسح محتويات هذا النطاق.

```csharp
public void ClearContents()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearContentsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات النموذجية لتوضيح عملية المسح
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue("Sample");
            worksheet.Cells["B2"].PutValue("Data");

            try
            {
                // أنشئ نطاقًا يغطي الخلايا A1:B2
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // اعرض محتويات النطاق قبل المسح
                Console.WriteLine("Before clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // استدعِ ClearContents لإزالة جميع القيم في النطاق
                range.ClearContents();

                // اعرض محتويات النطاق بعد المسح
                Console.WriteLine("\nAfter clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // احفظ المصنف
                workbook.Save("ClearContentsDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
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

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


