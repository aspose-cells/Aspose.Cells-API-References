---
title: "Enumeración PrintErrorsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.PrintErrorsType. Representa constantes de errores de impresión"
type: docs
url: /es/net/aspose.cells/printerrorstype/
---
## PrintErrorsType enumeration

Representa las constantes de errores de impresión.

```csharp
public enum PrintErrorsType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| PrintErrorsBlank | `0` | Representa no imprimir errores. |
| PrintErrorsDash | `1` | Representa imprimir errores como "--". |
| PrintErrorsDisplayed | `2` | Representa imprimir errores tal como se muestra. |
| PrintErrorsNA | `3` | Representa imprimir errores como "#N/A". |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintErrorsTypeDemo
    {
        public static void PrintErrorsTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder al PageSetup de la hoja de cálculo
            PageSetup pageSetup = worksheet.PageSetup;

            // Establecer diferentes tipos de error de impresión
            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            workbook.Save("PrintErrorsBlank.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            workbook.Save("PrintErrorsDash.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
            workbook.Save("PrintErrorsDisplayed.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsNA;
            workbook.Save("PrintErrorsNA.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


