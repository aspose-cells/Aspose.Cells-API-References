---
title: "Enum PowerQueryFormulaType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaType enum. Power query formülünün tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulatype/
---
## PowerQueryFormulaType enumeration

Power Query formülünün tipini temsil eder.

```csharp
public enum PowerQueryFormulaType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Formula | `0` | Formül power query formülü. |
| Function | `1` | Fonksiyon power query formülü. |
| Parameter | `2` | Parametre power query formülü. |

### Örnekler

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
                // PowerQueryFormulaType enum değerlerini göster
                PowerQueryFormulaType formulaType = PowerQueryFormulaType.Formula;
                PowerQueryFormulaType functionType = PowerQueryFormulaType.Function;
                PowerQueryFormulaType parameterType = PowerQueryFormulaType.Parameter;

                // Enum değerlerini ve sayısal temsillerini göster
                Console.WriteLine($"Formula type: {formulaType} ({(int)formulaType})");
                Console.WriteLine($"Function type: {functionType} ({(int)functionType})");
                Console.WriteLine($"Parameter type: {parameterType} ({(int)parameterType})");

                // Enum karşılaştırmasını göster
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

### Ayrıca Bakınız

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


