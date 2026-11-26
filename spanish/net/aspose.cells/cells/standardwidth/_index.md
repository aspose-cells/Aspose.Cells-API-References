---
title: "Cells.StandardWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo en unidades de caracteres"
type: docs
url: /es/net/aspose.cells/cells/standardwidth/
---
## Cells.StandardWidth property

Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres.

```csharp
public double StandardWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer el ancho estándar para columnas
            cells.StandardWidth = 18.25;

            // Mostrar el ancho estándar y el ancho real de la primera columna
            Console.WriteLine("Standard Width: " + cells.StandardWidth);
            Console.WriteLine("Column 0 Width: " + cells.GetColumnWidth(0));

            // Verificar que el ancho estándar se aplique (aproximadamente)
            if (Math.Abs(cells.GetColumnWidth(0) - cells.StandardWidth) > 1.0)
            {
                Console.WriteLine("Warning: Column width differs significantly from standard width");
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


