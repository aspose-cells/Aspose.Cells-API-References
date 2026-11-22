---
title: "فئة PowerQueryFormulaParameter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.QueryTables.PowerQueryFormulaParameter. يمثل معامل صيغة استعلام الطاقة"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulaparameter/
---
## PowerQueryFormulaParameter class

يمثل معامل صيغة Power Query.

```csharp
public class PowerQueryFormulaParameter : PowerQueryFormula
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | يحصل ويضبط وصف صيغة استعلام الطاقة.(موروث من [`PowerQueryFormula`](../powerqueryformula/).) |
| override [FormulaDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/) { get; } | يحصل على تعريف المعامل. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | يحصل على اسم المجموعة التي تحتوي على صيغة استعلام الطاقة.(موروث من [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | يحصل ويضبط اسم صيغة استعلام الطاقة.(موروث من [`PowerQueryFormula`](../powerqueryformula/).) |
| [ParameterDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/) { get; } | (**Obsolete.**) يحصل على تعريف المعامل. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | يحصل على جميع عناصر صيغة استعلام الطاقة.(موروث من [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulaparameter/type/) { get; } | يحصل على نوع صيغة استعلام الطاقة. |
| [Value](../../aspose.cells.querytables/powerqueryformulaparameter/value/) { get; set; } | يحصل على قيمة المعامل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterDemo
    {
        public static void PowerQueryFormulaParameterExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

            // الوصول إلى خاصية DataMashup في المصنف
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // الوصول إلى خاصية PowerQueryFormulas
                PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // الوصول إلى خاصية PowerQueryFormulaParameters
                PowerQueryFormulaParameterCollection powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // مثال على الاستخدام: تكرار عبر PowerQueryFormulas
                foreach (PowerQueryFormula formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // مثال على الاستخدام: التكرار عبر PowerQueryFormulaParameters
                foreach (PowerQueryFormulaParameter para in powerQueryFormulaParameters)
                {
                    // عرض تفاصيل المعامل
                    Console.WriteLine("Parameter Name: " + para.Name);
                    Console.WriteLine("Parameter Value: " + para.Value);

                    Console.WriteLine("Parameter Definition: " + para.ParameterDefinition);
                }
            }
            

            // احفظ المصنف
            workbook.Save("PowerQueryFormulaParameterExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


