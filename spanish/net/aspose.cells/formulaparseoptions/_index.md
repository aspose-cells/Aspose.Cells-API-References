---
title: "Clase FormulaParseOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FormulaParseOptions. Representa opciones al analizar una fórmula"
type: docs
url: /es/net/aspose.cells/formulaparseoptions/
---
## FormulaParseOptions class

Representa opciones al analizar una fórmula.

```csharp
public class FormulaParseOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [FormulaParseOptions](formulaparseoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CheckAddIn](../../aspose.cells/formulaparseoptions/checkaddin/) { get; set; } | Indica si se deben comprobar los complementos en los enlaces externos existentes del libro actual para funciones definidas por el usuario sin enlace externo. El valor predeterminado es true (si la función definida por el usuario coincide con un complemento en los enlaces externos existentes, se toma como el complemento). |
| [CustomFunctionDefinition](../../aspose.cells/formulaparseoptions/customfunctiondefinition/) { get; set; } | Definición para analizar funciones personalizadas. |
| [LocaleDependent](../../aspose.cells/formulaparseoptions/localedependent/) { get; set; } | Indica si la fórmula está formateada según la configuración regional. El valor predeterminado es false. |
| [Parse](../../aspose.cells/formulaparseoptions/parse/) { get; set; } | Indica si se debe analizar la fórmula proporcionada. El valor predeterminado es true. Si es false, la cadena de fórmula proporcionada se mantendrá tal cual en la celda hasta que el usuario llame a otros métodos para analizarla o se requieran los datos de la fórmula analizada por otras operaciones, como calcular fórmulas. |
| [R1C1Style](../../aspose.cells/formulaparseoptions/r1c1style/) { get; set; } | Indica si la fórmula usa el estilo de referencia R1C1. El valor predeterminado es false. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaParseOptionsDemo
    {
        public static void FormulaParseOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions
            {
                LocaleDependent = true,
                R1C1Style = false,
                CheckAddIn = true,
                Parse = true,
                CustomFunctionDefinition = null // Assuming no custom function definition for this example
            };

            // Agregar una fórmula a una celda usando las opciones
            Cell cell = worksheet.Cells["A1"];
            cell.SetFormula("=SUM(B1:B10)", options);

            // Guarda el libro de trabajo
            workbook.Save("FormulaParseOptionsExample.xlsx");
            workbook.Save("FormulaParseOptionsExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


