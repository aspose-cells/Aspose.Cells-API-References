---
title: "Enumeración PrintOrderType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.PrintOrderType. Representa constantes de orden de impresión"
type: docs
url: /es/net/aspose.cells/printordertype/
---
## PrintOrderType enumeration

Representa las constantes de orden de impresión.

```csharp
public enum PrintOrderType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DownThenOver | `0` | Abajo, luego a la derecha |
| OverThenDown | `1` | Derecha, luego abajo |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintOrderTypeDemo
    {
        public static void PrintOrderTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder al objeto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Establecer el orden de impresión a DownThenOver
            pageSetup.Order = PrintOrderType.DownThenOver;

            // Establecer algunas otras propiedades de configuración de página para demostración
            pageSetup.PrintArea = "A1:D10";
            pageSetup.PrintTitleRows = "$1:$1";
            pageSetup.PrintTitleColumns = "$A:$A";
            pageSetup.CenterHorizontally = true;
            pageSetup.CenterVertically = true;

            // Guarda el libro de trabajo
            workbook.Save("PrintOrderTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


