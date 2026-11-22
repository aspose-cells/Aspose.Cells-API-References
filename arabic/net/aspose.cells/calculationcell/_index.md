---
title: "الفئة CalculationCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CalculationCell. تمثل البيانات المتعلقة بالحساب لخلية واحدة يتم حسابها"
type: docs
url: /ar/net/aspose.cells/calculationcell/
---
## CalculationCell class

يمثل البيانات المتعلقة بالحساب لخلية واحدة يتم حسابها.

```csharp
public class CalculationCell
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Cell](../../aspose.cells/calculationcell/cell/) { get; } | يحصل على كائن Cell الذي يتم حسابه. |
| [CellColumn](../../aspose.cells/calculationcell/cellcolumn/) { get; } | يحصل على فهرس العمود للخلية. |
| [CellRow](../../aspose.cells/calculationcell/cellrow/) { get; } | يحصل على فهرس الصف للخلية. |
| [Workbook](../../aspose.cells/calculationcell/workbook/) { get; } | يحصل على كائن Workbook. |
| [Worksheet](../../aspose.cells/calculationcell/worksheet/) { get; } | يحصل على كائن Worksheet الذي توجد فيه الخلية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetCalculatedValue](../../aspose.cells/calculationcell/setcalculatedvalue/)(object) | يضبط القيمة المحسوبة للخلية. |

### ملاحظات

يجب على المستخدم عدم تغيير أي بيانات في الـWorkbook أثناء عملية حساب الصيغة، وإلا قد يحدث نتيجة غير متوقعة أو استثناء. لذلك، جميع الكائنات التي توفرها هذه الفئة (مثل كائن Cell من [`Cell`](./cell/)) مخصصة للقراءة فقط.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CellsClassCalculationCellDemo
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

                // عرض الخصائص الأساسية
                Console.WriteLine($"Cell Row: {calcCell.CellRow}");
                Console.WriteLine($"Cell Column: {calcCell.CellColumn}");
                Console.WriteLine($"Cell Value: {calcCell.Cell.Value}");
                Console.WriteLine($"Workbook Name: {calcCell.Workbook.FileName}");
                Console.WriteLine($"Worksheet Name: {calcCell.Worksheet.Name}");

                // احفظ المصنف
                workbook.Save("CalculationCellDemo.xlsx");
                Console.WriteLine("CalculationCell demonstration completed successfully.");
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


