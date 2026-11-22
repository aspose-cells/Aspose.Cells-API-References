---
title: "تعداد PowerQueryFormulaType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.QueryTables.PowerQueryFormulaType. يمثل نوع صيغة استعلام الطاقة"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulatype/
---
## PowerQueryFormulaType enumeration

يمثل نوع صيغة Power Query.

```csharp
public enum PowerQueryFormulaType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Formula | `0` | صيغة استعلام الطاقة. |
| Function | `1` | دالة استعلام الطاقة. |
| Parameter | `2` | معامل استعلام الطاقة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.QueryTables;
    using System;

    public class QueryTablesClassPowerQueryFormulaTypeDemo
    {
        public static void Run()
        {
            try
            {
                // عرض جميع قيم التعداد لـ PowerQueryFormulaType
                PowerQueryFormulaType formulaType = PowerQueryFormulaType.Formula;
                PowerQueryFormulaType functionType = PowerQueryFormulaType.Function;
                PowerQueryFormulaType parameterType = PowerQueryFormulaType.Parameter;

                // عرض قيم التعداد وتمثيلاتها الرقمية
                Console.WriteLine($"Formula type: {formulaType} ({(int)formulaType})");
                Console.WriteLine($"Function type: {functionType} ({(int)functionType})");
                Console.WriteLine($"Parameter type: {parameterType} ({(int)parameterType})");

                // عرض مقارنة التعداد
                if (formulaType == PowerQueryFormulaType.Formula)
                {
                    Console.WriteLine("Successfully identified Formula type");
                }

                if (functionType == PowerQueryFormulaType.Function)
                {
                    Console.WriteLine("Successfully identified Function type");
                }

                if (parameterType == PowerQueryFormulaType.Parameter)
                {
                    Console.WriteLine("Successfully identified Parameter type");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormulaType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


