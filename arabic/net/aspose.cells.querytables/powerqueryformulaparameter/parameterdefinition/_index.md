---
title: "PowerQueryFormulaParameter.ParameterDefinition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormulaParameter. تحصل على تعريف المعامل"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/
---
## PowerQueryFormulaParameter.ParameterDefinition property

يحصل على تعريف المعامل.

```csharp
[Obsolete("Use PowerQueryFormulaParameter.FormulaDefinition property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ParameterDefinition { get; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PowerQueryFormulaParameter.FormulaDefinition. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من نوفمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyParameterDefinitionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى خاصية DataMashup في المصنف
                DataMashup dataMashup = workbook.DataMashup;

                if (dataMashup != null)
                {
                    // الوصول إلى مجموعة PowerQueryFormulaParameters
                    PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                    // التكرار عبر المعاملات لعرض ParameterDefinition
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // عرض قيمة خاصية ParameterDefinition (خاصية للقراءة فقط)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Parameter Definition: {parameter.ParameterDefinition}");
                        Console.WriteLine($"Formula Definition: {parameter.FormulaDefinition}");
                        Console.WriteLine($"Parameter Value: {parameter.Value}");
                        Console.WriteLine("----------------------------------------");
                    }

                    if (parameters.Count == 0)
                    {
                        Console.WriteLine("No PowerQueryFormulaParameter instances found in the workbook.");
                    }
                }
                else
                {
                    Console.WriteLine("No DataMashup available in the workbook.");
                }

                // احفظ المصنف
                workbook.Save("ParameterDefinitionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


