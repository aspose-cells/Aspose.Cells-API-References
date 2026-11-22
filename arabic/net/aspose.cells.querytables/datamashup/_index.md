---
title: "الفئة DataMashup"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.QueryTables.DataMashup. تمثل بيانات الماش أب"
type: docs
url: /ar/net/aspose.cells.querytables/datamashup/
---
## DataMashup class

يمثل بيانات الدمج.

```csharp
public class DataMashup
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [PowerQueryFormulaParameters](../../aspose.cells.querytables/datamashup/powerqueryformulaparameters/) { get; } | (**مهمل.**) يحصل على معلمات صيغة استعلام الطاقة. |
| [PowerQueryFormulas](../../aspose.cells.querytables/datamashup/powerqueryformulas/) { get; } | يحصل على جميع صيغ Power Query. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class DataMashupDemo
    {
        public static void DataMashupExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى خاصية DataMashup في المصنف
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null )
            {
                // الوصول إلى خاصية PowerQueryFormulas
                var powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // الوصول إلى خاصية PowerQueryFormulaParameters
                var powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // مثال على الاستخدام: تكرار عبر PowerQueryFormulas
                foreach (var formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // مثال على الاستخدام: التكرار عبر PowerQueryFormulaParameters
                foreach (var parameter in powerQueryFormulaParameters)
                {
                    Console.WriteLine(parameter.Name);
                }
            }
            

            // احفظ المصنف
            workbook.Save("DataMashupExample.xlsx");
            workbook.Save("DataMashupExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


