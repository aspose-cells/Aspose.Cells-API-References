---
title: "Enumeración PowerQueryFormulaType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.QueryTables.PowerQueryFormulaType. Representa el tipo de fórmula de Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulatype/
---
## PowerQueryFormulaType enumeration

Representa el tipo de fórmula Power Query

```csharp
public enum PowerQueryFormulaType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Formula | `0` | Fórmula de Power Query. |
| Function | `1` | Función de Power Query. |
| Parameter | `2` | Parámetro de Power Query. |

### Ejemplos

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
                // Demostrar todos los valores de enumeración de PowerQueryFormulaType
                PowerQueryFormulaType formulaType = PowerQueryFormulaType.Formula;
                PowerQueryFormulaType functionType = PowerQueryFormulaType.Function;
                PowerQueryFormulaType parameterType = PowerQueryFormulaType.Parameter;

                // Mostrar los valores de enumeración y sus representaciones numéricas
                Console.WriteLine($"Formula type: {formulaType} ({(int)formulaType})");
                Console.WriteLine($"Function type: {functionType} ({(int)functionType})");
                Console.WriteLine($"Parameter type: {parameterType} ({(int)parameterType})");

                // Demostrar la comparación de enumeraciones
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

### Ver también

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


