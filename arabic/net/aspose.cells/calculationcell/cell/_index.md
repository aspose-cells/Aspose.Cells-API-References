---
title: "CalculationCell.Cell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationCell. تحصل على كائن Cell الذي يتم حسابه"
type: docs
url: /ar/net/aspose.cells/calculationcell/cell/
---
## CalculationCell.Cell property

يحصل على كائن Cell الذي يتم حسابه.

```csharp
public Cell Cell { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyCellDemo
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

                // عرض قيمة خاصية Cell
                Console.WriteLine("Cell Name: " + calcCell.Cell.Name);
                Console.WriteLine("Cell Value: " + calcCell.Cell.Value);
                Console.WriteLine("Cell StringValue: " + calcCell.Cell.StringValue);
                Console.WriteLine("Cell Row: " + calcCell.Cell.Row);
                Console.WriteLine("Cell Column: " + calcCell.Cell.Column);
                Console.WriteLine("Cell IsFormula: " + calcCell.Cell.IsFormula);

                // أظهر الخصائص المرتبطة للسياق
                Console.WriteLine("CellRow: " + calcCell.CellRow);
                Console.WriteLine("CellColumn: " + calcCell.CellColumn);

                // احفظ المصنف
                workbook.Save("CellDemo.xlsx");
                Console.WriteLine("Cell property demonstration completed successfully.");
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

* class [Cell](../../cell/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


