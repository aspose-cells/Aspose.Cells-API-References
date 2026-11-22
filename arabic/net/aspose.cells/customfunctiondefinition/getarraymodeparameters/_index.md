---
title: "CustomFunctionDefinition.GetArrayModeParameters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CustomFunctionDefinition. تحصل على مؤشرات معلمات الدالة المخصصة المعطاة التي تحتاج إلى حسابها في وضع المصفوفة"
type: docs
url: /ar/net/aspose.cells/customfunctiondefinition/getarraymodeparameters/
---
## CustomFunctionDefinition.GetArrayModeParameters method

يحصل على مؤشرات معلمات الدالة المخصصة المعطاة التي تحتاج إلى حسابها في وضع المصفوفة.

```csharp
public virtual int[] GetArrayModeParameters(string functionName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| functionName | String | اسم الدالة المخصصة. |

### قيمة الإرجاع

مؤشرات المعلمات التي تحتاج إلى حسابها في وضع المصفوفة للدالة المخصصة المعطاة. القيمة الافتراضية هي null، لا توجد معلمة تحتاج إلى حسابها في وضع المصفوفة للدالة المخصصة.

### ملاحظات

لتعبير يحتاج إلى حسابه، مع أخذ A:A+B:B كمثال: بشكل عام في وضع القيمة سيتم حسابه إلى قيمة واحدة وفقًا لقاعدة الخلية الحالية. ولكن في وضع المصفوفة، سيتم حساب جميع القيم A1+B1، A2+B2، A3+B3، ... واستخدامها في الحساب.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionMethodGetArrayModeParametersWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائن من CustomFunctionDefinition
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();

            try
            {
                // استدعاء GetArrayModeParameters مع معامل اسم الدالة
                string functionName = "SUM";
                int[] result = customFunction.GetArrayModeParameters(functionName);

                // اعرض النتيجة
                if (result != null)
                {
                    Console.WriteLine("Array mode parameters for function '{0}':", functionName);
                    foreach (int param in result)
                    {
                        Console.WriteLine(param);
                    }
                }
                else
                {
                    Console.WriteLine("No array mode parameters defined for function '{0}'", functionName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetArrayModeParameters method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("CustomFunctionDefinitionGetArrayModeParametersDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CustomFunctionDefinition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


