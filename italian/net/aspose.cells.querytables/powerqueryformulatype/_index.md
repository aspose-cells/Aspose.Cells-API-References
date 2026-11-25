---
title: "Enum PowerQueryFormulaType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaType enum. Rappresenta il tipo di formula power query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulatype/
---
## PowerQueryFormulaType enumeration

Rappresenta il tipo di formula Power Query.

```csharp
public enum PowerQueryFormulaType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Formula | `0` | Formula power query. |
| Function | `1` | Funzione power query. |
| Parameter | `2` | Parametro power query. |

### Esempi

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
                // Dimostra tutti i valori enum di PowerQueryFormulaType
                PowerQueryFormulaType formulaType = PowerQueryFormulaType.Formula;
                PowerQueryFormulaType functionType = PowerQueryFormulaType.Function;
                PowerQueryFormulaType parameterType = PowerQueryFormulaType.Parameter;

                // Visualizza i valori enum e le loro rappresentazioni numeriche
                Console.WriteLine($"Formula type: {formulaType} ({(int)formulaType})");
                Console.WriteLine($"Function type: {functionType} ({(int)functionType})");
                Console.WriteLine($"Parameter type: {parameterType} ({(int)parameterType})");

                // Dimostra il confronto enum
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

### Vedi anche

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


