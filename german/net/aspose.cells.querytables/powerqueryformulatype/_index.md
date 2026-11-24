---
title: "Enum PowerQueryFormulaType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaType enum. Stellt den Typ der Power‑Query‑Formel dar"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulatype/
---
## PowerQueryFormulaType enumeration

Stellt den Typ einer Power‑Query‑Formel dar.

```csharp
public enum PowerQueryFormulaType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Formula | `0` | Formel Power‑Query‑Formel. |
| Function | `1` | Funktion Power‑Query‑Formel. |
| Parameter | `2` | Parameter Power‑Query‑Formel. |

### Beispiele

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
                // Demonstration aller Enum‑Werte von PowerQueryFormulaType
                PowerQueryFormulaType formulaType = PowerQueryFormulaType.Formula;
                PowerQueryFormulaType functionType = PowerQueryFormulaType.Function;
                PowerQueryFormulaType parameterType = PowerQueryFormulaType.Parameter;

                // Enum‑Werte und deren numerische Darstellungen anzeigen
                Console.WriteLine($"Formula type: {formulaType} ({(int)formulaType})");
                Console.WriteLine($"Function type: {functionType} ({(int)functionType})");
                Console.WriteLine($"Parameter type: {parameterType} ({(int)parameterType})");

                // Demonstration des Enum‑Vergleichs
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

### Siehe auch

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


