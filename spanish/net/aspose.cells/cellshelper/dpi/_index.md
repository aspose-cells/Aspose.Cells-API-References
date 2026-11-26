---
title: "CellsHelper.DPI"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsHelper. Obtiene el DPI de la máquina"
type: docs
url: /es/net/aspose.cells/cellshelper/dpi/
---
## CellsHelper.DPI property

Obtiene los DPI de la máquina.

```csharp
public static double DPI { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyDPIDemo
    {
        public static void Run()
        {
            // Establecer y mostrar el DPI actual
            Console.WriteLine("Original DPI: " + CellsHelper.DPI);
            
            // Cambiar la configuración de DPI
            CellsHelper.DPI = 300;
            Console.WriteLine("New DPI: " + CellsHelper.DPI);

            // Crear un nuevo libro de trabajo y guardar con diferentes configuraciones de DPI
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar una forma de ejemplo para demostrar el efecto del DPI
            sheet.Shapes.AddRectangle(1, 1, 10, 10, 100, 100);

            // Guardar con la configuración de DPI actual
            workbook.Save("output_with_dpi_300.xlsx");

            // Cambiar DPI y guardar de nuevo
            CellsHelper.DPI = 96;
            workbook.Save("output_with_dpi_96.xlsx");
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


