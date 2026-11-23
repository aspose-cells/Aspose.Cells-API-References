---
title: "Enum PowerQueryFormulaType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "enum Aspose.Cells.QueryTables.PowerQueryFormulaType. Représente le type de formule Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulatype/
---
## PowerQueryFormulaType enumeration

Représente le type de formule Power Query.

```csharp
public enum PowerQueryFormulaType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Formula | `0` | Formule Power Query. |
| Function | `1` | Fonction Power Query. |
| Parameter | `2` | Paramètre Power Query. |

### Exemples

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
                // Démontrer toutes les valeurs d'énumération de PowerQueryFormulaType
                PowerQueryFormulaType formulaType = PowerQueryFormulaType.Formula;
                PowerQueryFormulaType functionType = PowerQueryFormulaType.Function;
                PowerQueryFormulaType parameterType = PowerQueryFormulaType.Parameter;

                // Afficher les valeurs d'énumération et leurs représentations numériques
                Console.WriteLine($"Formula type: {formulaType} ({(int)formulaType})");
                Console.WriteLine($"Function type: {functionType} ({(int)functionType})");
                Console.WriteLine($"Parameter type: {parameterType} ({(int)parameterType})");

                // Démontrer la comparaison d'énumération
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

### Voir aussi

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


