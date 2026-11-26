---
title: "Clase CustomFunctionDefinition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CustomFunctionDefinition. Definición de función personalizada para calcular con el motor personalizado del usuario"
type: docs
url: /es/net/aspose.cells/customfunctiondefinition/
---
## CustomFunctionDefinition class

Definición de una función personalizada para calcular con el motor personalizado del usuario.

```csharp
public class CustomFunctionDefinition
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CustomFunctionDefinition](customfunctiondefinition/)() | El constructor predeterminado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [GetArrayModeParameters](../../aspose.cells/customfunctiondefinition/getarraymodeparameters/)(string) | Obtiene los índices de los parámetros de la función personalizada dada que deben calcularse en modo de matriz. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionDemo
    {
        public static void CustomFunctionDefinitionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una nueva instancia de CustomFunctionDefinition
            CustomFunctionDefinition customFunctionDefinition = new CustomFunctionDefinition();

            // Crear una nueva instancia de FormulaParseOptions y establecer la CustomFunctionDefinition
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunctionDefinition
            };

            // Agregar una hoja de cálculo al libro de trabajo
            Worksheet worksheet = workbook.Worksheets[0];

            // Definir una fórmula personalizada
            string customFormula = "=MY_CUSTOM_FUNCTION(A1, B1)";

            // Analizar la fórmula personalizada usando FormulaParseOptions
            worksheet.Cells["C1"].Formula = customFormula;
            worksheet.Cells["C1"].SetFormula(customFormula, formulaParseOptions);

            // Guarda el libro de trabajo
            workbook.Save("CustomFunctionDefinitionExample.xlsx");
            workbook.Save("CustomFunctionDefinitionExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


