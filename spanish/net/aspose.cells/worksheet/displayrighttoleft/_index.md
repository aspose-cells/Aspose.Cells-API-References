---
title: "Worksheet.DisplayRightToLeft"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/worksheet/displayrighttoleft/
---
## Worksheet.DisplayRightToLeft property

Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. El valor predeterminado es false.

```csharp
public bool DisplayRightToLeft { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyDisplayRightToLeftDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establezca la visualización de derecha a izquierda
            worksheet.DisplayRightToLeft = true;
            
            // Guarda el libro de trabajo
            workbook.Save("output.ods");
            
            // Vuelva a cargar el libro de trabajo para verificar la configuración
            Workbook loadedWorkbook = new Workbook("output.ods");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            Console.WriteLine("DisplayRightToLeft: " + loadedWorksheet.DisplayRightToLeft);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


