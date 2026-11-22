---
title: "CalculationCell.CellRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationCell. تحصل على فهرس الصف للخلية"
type: docs
url: /ar/net/aspose.cells/calculationcell/cellrow/
---
## CalculationCell.CellRow property

يحصل على فهرس الصف للخلية.

```csharp
public int CellRow { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyCellRowDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // إنشاء كائن CalculationCell باستخدام الانعكاس لأن المُنشئ غير عام
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // اعرض قيمة خاصية CellRow
                Console.WriteLine("CellRow value: " + calcCell.CellRow);

                // أظهر الخصائص المرتبطة للسياق
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);
                Console.WriteLine("Cell Value: " + calcCell.Cell.Value);

                // احفظ المصنف
                workbook.Save("CellRowDemo.xlsx");
                Console.WriteLine("CellRow property demonstration completed successfully.");
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

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


