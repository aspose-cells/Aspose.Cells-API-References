---
title: "PowerQueryFormulaParameter.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormulaParameter. تحصل على قيمة المعامل"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulaparameter/value/
---
## PowerQueryFormulaParameter.Value property

يحصل على قيمة المعامل.

```csharp
public string Value { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyValueDemo
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

                    // التكرار عبر المعاملات لعرض خاصية Value
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // عرض القيمة الحالية لخاصية Value (عملية قراءة)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Current Value: {parameter.Value}");

                        // نظرًا لأن Value قابلة للقراءة والكتابة، يتم توضيح تعيين قيمة جديدة
                        string newValue = "UpdatedValue_" + Guid.NewGuid().ToString();
                        parameter.Value = newValue;
                        Console.WriteLine($"Updated Value: {parameter.Value}");
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
                workbook.Save("ValueDemo.xlsx");
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


