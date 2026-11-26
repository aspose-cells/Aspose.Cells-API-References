---
title: "DeleteBlankOptions.DrawingsAsBlank"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DeleteBlankOptions. Indica si los objetos relacionados con dibujos, como imágenes, formas, gráficos... se considerarán en blanco. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/deleteblankoptions/drawingsasblank/
---
## DeleteBlankOptions.DrawingsAsBlank property

Indica si los objetos relacionados con dibujos, como imágenes, formas, gráficos..., se considerarán en blanco. El valor predeterminado es true.

```csharp
public bool DrawingsAsBlank { get; set; }
```

### Observaciones

Al establecer esta propiedad como false, todas las filas/columnas cubiertas por objetos de dibujo no se considerarán en blanco y no se eliminarán.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyDrawingsAsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data");
            worksheet.Cells["B1"].PutValue("");
            worksheet.Cells["B2"].PutValue("");

            // Agregue un objeto de dibujo para probar el comportamiento de DrawingsAsBlank
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);

            // Eliminar columnas en blanco con DrawingsAsBlank = false (preserva los dibujos)
            worksheet.Cells.DeleteBlankColumns(new DeleteBlankOptions { DrawingsAsBlank = false });

            Console.WriteLine("Drawing preserved count: " + worksheet.Shapes.Count);
        }
    }
}
```

### Ver también

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


