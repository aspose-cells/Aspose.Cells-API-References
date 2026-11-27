---
title: "Enum PowerQueryFormulaType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaType‑enum. Representerar typen av power query‑formel"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulatype/
---
## PowerQueryFormulaType enumeration

Representerar typen av Power Query‑formel.

```csharp
public enum PowerQueryFormulaType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Formula | `0` | Formel power query‑formel. |
| Function | `1` | Funktion power query‑formel. |
| Parameter | `2` | Parameter power query‑formel. |

### Exempel

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
                // Demonstrera alla enum‑värden för PowerQueryFormulaType
                PowerQueryFormulaType formulaType = PowerQueryFormulaType.Formula;
                PowerQueryFormulaType functionType = PowerQueryFormulaType.Function;
                PowerQueryFormulaType parameterType = PowerQueryFormulaType.Parameter;

                // Visa enum‑värden och deras numeriska representationer
                Console.WriteLine($"Formula type: {formulaType} ({(int)formulaType})");
                Console.WriteLine($"Function type: {functionType} ({(int)functionType})");
                Console.WriteLine($"Parameter type: {parameterType} ({(int)parameterType})");

                // Demonstrera enum‑jämförelse
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

### Se även

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


