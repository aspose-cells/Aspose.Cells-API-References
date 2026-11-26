---
title: "FormulaParseOptions.CustomFunctionDefinition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaParseOptions. Definición para analizar funciones personalizadas"
type: docs
url: /es/net/aspose.cells/formulaparseoptions/customfunctiondefinition/
---
## FormulaParseOptions.CustomFunctionDefinition property

Definición para analizar funciones personalizadas.

```csharp
public CustomFunctionDefinition CustomFunctionDefinition { get; set; }
```

### Observaciones

Para algunos requisitos especiales, como al calcular una función personalizada en el motor personalizado del usuario, algunos de sus parámetros deben calcularse en modo matriz; al usar esta propiedad se pueden marcar esos parámetros como modo matriz al analizar la fórmula. De lo contrario, el usuario deberá actualizar esas funciones personalizadas más tarde mediante [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) para obtener el mismo resultado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCustomFunctionDefinitionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear definición de función personalizada
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();
            
            // Configurar opciones de análisis de fórmula con función personalizada
            FormulaParseOptions options = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunction,
                Parse = true
            };

            // Establecer datos de muestra
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);

            // Utilizar función personalizada en la fórmula
            string formula = "=MY_CUSTOM_FUNCTION(A1, B1)";
            worksheet.Cells["C1"].SetFormula(formula, options);

            // Calcular el libro para demostrar el procesamiento de la función personalizada
            workbook.CalculateFormula();

            // Guardar resultado
            workbook.Save("CustomFunctionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


