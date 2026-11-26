---
title: "Clase PowerQueryFormulaParameter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.QueryTables.PowerQueryFormulaParameter. Representa el parámetro de la fórmula de Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulaparameter/
---
## PowerQueryFormulaParameter class

Representa el parámetro de la fórmula Power Query.

```csharp
public class PowerQueryFormulaParameter : PowerQueryFormula
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Obtiene y establece la descripción de la fórmula de Power Query.(Heredado de [`PowerQueryFormula`](../powerqueryformula/).) |
| override [FormulaDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/) { get; } | Obtiene la definición del parámetro. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Obtiene el nombre del grupo que contiene esta fórmula de Power Query.(Heredado de [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Obtiene y establece el nombre de la fórmula de Power Query.(Heredado de [`PowerQueryFormula`](../powerqueryformula/).) |
| [ParameterDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/) { get; } | (**Obsolete.**) Obtiene la definición del parámetro. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Obtiene todos los elementos de la fórmula de Power Query.(Heredado de [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulaparameter/type/) { get; } | Obtiene el tipo de la fórmula de Power Query. |
| [Value](../../aspose.cells.querytables/powerqueryformulaparameter/value/) { get; set; } | Obtiene el valor del parámetro. |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

            // Acceder a la propiedad DataMashup del libro de trabajo
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Acceder a la propiedad PowerQueryFormulas
                PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Acceder a la propiedad PowerQueryFormulaParameters
                PowerQueryFormulaParameterCollection powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Ejemplo de uso: Iterar a través de PowerQueryFormulas
                foreach (PowerQueryFormula formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Ejemplo de uso: iterar a través de PowerQueryFormulaParameters
                foreach (PowerQueryFormulaParameter para in powerQueryFormulaParameters)
                {
                    // Mostrar los detalles del parámetro
                    Console.WriteLine("Parameter Name: " + para.Name);
                    Console.WriteLine("Parameter Value: " + para.Value);

                    Console.WriteLine("Parameter Definition: " + para.ParameterDefinition);
                }
            }
            

            // Guarda el libro de trabajo
            workbook.Save("PowerQueryFormulaParameterExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


