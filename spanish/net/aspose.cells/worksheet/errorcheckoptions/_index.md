---
title: "Worksheet.ErrorCheckOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene la configuración de comprobación de errores aplicada a ciertos rangos"
type: docs
url: /es/net/aspose.cells/worksheet/errorcheckoptions/
---
## Worksheet.ErrorCheckOptions property

Obtiene la configuración de comprobación de errores aplicada a ciertos rangos.

```csharp
public ErrorCheckOptionCollection ErrorCheckOptions { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyErrorCheckOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Habilite las opciones de comprobación de errores
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            ErrorCheckOption option = options[0]; // Properly access first option using indexer
            option.SetErrorCheck(ErrorCheckType.TextDate, true);
            option.AddRange(CellArea.CreateCellArea(0, 0, 10, 10));
            
            // Obtenga el recuento de rangos para la opción
            int rangeCount = option.GetCountOfRange();
            Console.WriteLine("Number of ranges in ErrorCheckOption: " + rangeCount);
            
            // Guarda el libro de trabajo
            workbook.Save("ErrorCheckOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ErrorCheckOptionCollection](../../errorcheckoptioncollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


