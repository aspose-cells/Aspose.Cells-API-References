---
title: "Workbook.UpdateCustomFunctionDefinition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تقوم بتحديث تعريف الدوال المخصصة"
type: docs
url: /ar/net/aspose.cells/workbook/updatecustomfunctiondefinition/
---
## Workbook.UpdateCustomFunctionDefinition method

يحدّث تعريف الدوال المخصصة.

```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| التعريف | CustomFunctionDefinition | تعريف خاص للدوال المخصصة لتلبية متطلبات المستخدم الخاصة. |

### ملاحظات

يمكن استخدام هذه الطريقة لبعض السيناريوهات الخاصة. على سبيل المثال، إذا كان المستخدم يحتاج إلى حساب بعض معلمات بعض الدوال المخصصة في وضع المصفوفة، يمكن للمستخدم تقديم تعريفه الخاص مع تنفيذ [`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) لتلك الدوال. بعد تحديث بيانات الصيغ، سيتم حساب تلك المعلمات المحددة في وضع المصفوفة تلقائيًا عند حساب الدوال المخصصة المقابلة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUpdateCustomFunctionDefinitionWithCustomFunctionDDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // أضف بيانات تجريبية
            sheet.Cells["B1"].PutValue(1);
            sheet.Cells["C1"].PutValue(2);
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["C2"].PutValue(8);

            // أنشئ محرك حساب مخصص
            var customEngine = new MyCustomCalculationEngine();
            
            // تعيين خيارات الحساب مع محرك مخصص
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };

            // تحديث تعريف الدالة المخصصة
            wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());

            // تعيين الصيغة باستخدام الدالة المخصصة
            sheet.Cells["A1"].Formula = "=MYFUNC(B:B+C:C)";
            
            // حساب الصيغ
            wb.CalculateFormula(options);

            // أخرج النتيجة.
            Console.WriteLine("Custom function result: " + sheet.Cells["A1"].Value);
        }
    }

    public class MyCustomFunctionDefinition : CustomFunctionDefinition
    {
        public override int[] GetArrayModeParameters(string functionName)
        {
            // إرجاع مؤشرات المعلمات التي يجب معالجتها في وضع المصفوفة
            return new int[] { 0 }; // First parameter is array mode
        }
    }

    public class MyCustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYFUNC")
            {
                double sum = 0;
                var paramValue = data.GetParamValue(0);
                
                if (paramValue is object[,] arrayValue)
                {
                    foreach (var val in arrayValue)
                    {
                        if (val != null)
                        {
                            sum += Convert.ToDouble(val);
                        }
                    }
                }
                else
                {
                    sum += Convert.ToDouble(paramValue);
                }
                data.CalculatedValue = sum * 2; // Custom calculation logic
            }
        }
    }
}
```

### انظر أيضًا

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


