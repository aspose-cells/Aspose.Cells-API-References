---
title: "PowerQueryFormulaParameter.FormulaDefinition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormulaParameter. تحصل على تعريف المعامل"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/
---
## PowerQueryFormulaParameter.FormulaDefinition property

يحصل على تعريف المعامل.

```csharp
public override string FormulaDefinition { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyFormulaDefinitionDemo
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

                    // التكرار عبر المعلمات لإظهار FormulaDefinition
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // عرض قيمة الخاصية FormulaDefinition (خاصية للقراءة فقط)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
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
                workbook.Save("FormulaDefinitionDemo.xlsx");
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


