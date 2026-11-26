---
title: "Clase CellRichValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CellRichValue. Representa el valor enriquecido de la celda"
type: docs
url: /es/net/aspose.cells/cellrichvalue/
---
## CellRichValue class

Representa el valor enriquecido de la celda.

```csharp
public abstract class CellRichValue
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [AltText](../../aspose.cells/cellrichvalue/alttext/) { get; set; } | Obtiene el texto alternativo asociado a la imagen. |
| virtual [ErrorValue](../../aspose.cells/cellrichvalue/errorvalue/) { get; } | Obtiene el tipo de valor de error de la celda. |
| virtual [Image](../../aspose.cells/cellrichvalue/image/) { get; } | Obtiene los datos de la imagen de la celda. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCellRichValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer un valor enriquecido en la celda A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Rich Value");
            
            // Obtener el valor enriquecido de la celda A1
            CellRichValue richValue = cell.GetRichValue();
            
            // Mostrar las propiedades del valor enriquecido
            Console.WriteLine("Rich Value: " + richValue.ToString());
            
            // Guarda el libro de trabajo
            workbook.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


