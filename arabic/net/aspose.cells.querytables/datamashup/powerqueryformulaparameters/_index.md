---
title: "DataMashup.PowerQueryFormulaParameters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataMashup. يحصل على معلمات صيغة Power Query"
type: docs
url: /ar/net/aspose.cells.querytables/datamashup/powerqueryformulaparameters/
---
## DataMashup.PowerQueryFormulaParameters property

يحصل على معلمات صيغة Power Query.

```csharp
[Obsolete("Use DataMashup.PowerQueryFormulas property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PowerQueryFormulaParameterCollection PowerQueryFormulaParameters { get; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية DataMashup.PowerQueryFormulas. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ نوفمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulaParametersDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى خاصية DataMashup
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // الوصول إلى PowerQueryFormulaParameters
                PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                // عرض عدد المعلمات
                Console.WriteLine($"Number of parameters: {parameters.Count}");

                // التكرار عبر المعلمات إذا وجدت أي منها
                foreach (PowerQueryFormulaParameter parameter in parameters)
                {
                    Console.WriteLine($"Parameter Name: {parameter.Name}, Value: {parameter.Value}");
                }
            }

            // احفظ المصنف
            workbook.Save("DataMashupDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormulaParameterCollection](../../powerqueryformulaparametercollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


