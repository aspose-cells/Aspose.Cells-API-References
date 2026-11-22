---
title: "CalculationData.Cell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationData. تحصل على كائن Cell حيث تكون الدالة"
type: docs
url: /ar/net/aspose.cells/calculationdata/cell/
---
## CalculationData.Cell property

يحصل على كائن Cell حيث توجد الدالة.

```csharp
public Cell Cell { get; }
```

### ملاحظات

عند حساب صيغة دون تعيينها إلى خلية، مثلًا باستخدام [`CalculateFormula`](../../worksheet/calculateformula/)، سيتم حساب الصيغة كما لو تم تعيينها إلى الخلية A1، لذا فإن كلًا من [`CellRow`](../cellrow/) و[`CellColumn`](../cellcolumn/) يساويان 0. ومع ذلك، قد لا تكون الخلية A1 في ورقة العمل مُنشأة. لذلك في مثل هذه الحالة ستكون هذه الخاصية فارغة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // إضافة بعض البيانات لجعل المثال ذو معنى
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // إنشاء خيارات الحساب باستخدام محرك مخصص
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellDemoEngine();

                // حساب الصيغ مع خيارات
                workbook.CalculateFormula(options);

                // اعرض النتيجة
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // حفظ النتيجة
                workbook.Save("CellDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // الوصول إلى خاصية Cell للقراءة فقط
                Cell cell = data.Cell;
                Console.WriteLine($"Function is in cell: {cell.Name}");
                Console.WriteLine($"Cell value: {cell.StringValue}");
                Console.WriteLine($"Cell row: {cell.Row}, column: {cell.Column}");

                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


