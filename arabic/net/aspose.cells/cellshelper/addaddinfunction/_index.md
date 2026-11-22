---
title: "CellsHelper.AddAddInFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. إضافة وظيفة addin"
type: docs
url: /ar/net/aspose.cells/cellshelper/addaddinfunction/
---
## CellsHelper.AddAddInFunction method

إضافة وظيفة addin.

```csharp
[Obsolete("Use WorksheetCollection.RegisterAddInFunction() methods instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static void AddAddInFunction(string function, int minCountOfParameters, 
    int maxCountOfParameters, ParameterType[] paramersType, ParameterType functionValueType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دالة | String | اسم الدالة. |
| minCountOfParameters | Int32 | الحد الأدنى لعدد المعلمات التي تتطلبها هذه الدالة |
| maxCountOfParameters | Int32 | الحد الأقصى لعدد المعلمات التي تسمح بها هذه الدالة. |
| paramersType | ParameterType[] | نوع المعلمات المتوقعة للدالة |
| functionValueType | ParameterType | نوع قيمة الدالة. |

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طرق WorksheetCollection.RegisterAddInFunction(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يناير 2022. تقدم Aspose اعتذارًا عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodAddAddInFunctionWithStringInt32Int32ParameterTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // تحديد المعلمات لـ AddAddInFunction
                string functionName = "CUSTOMFUNCTION";
                int minParams = 2;
                int maxParams = 4;
                ParameterType[] paramTypes = new ParameterType[] { ParameterType.Value, ParameterType.Reference };
                ParameterType returnType = ParameterType.Value;

                // استدعِ طريقة AddAddInFunction
                CellsHelper.AddAddInFunction(functionName, minParams, maxParams, paramTypes, returnType);

                // استخدام الدالة المخصصة في خلية
                worksheet.Cells["A1"].Formula = "=CUSTOMFUNCTION(5,B2)";
                worksheet.Cells["B2"].Value = 10;

                // حساب الصيغ
                workbook.CalculateFormula();

                Console.WriteLine("AddAddInFunction executed successfully. Custom function added and used in A1.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAddInFunction method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("AddAddInFunctionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ParameterType](../../parametertype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


