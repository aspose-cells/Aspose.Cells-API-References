---
title: "Column.Width"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Column. Obtiene y establece el ancho de la columna en unidades de caracteres"
type: docs
url: /es/net/aspose.cells/column/width/
---
## Column.Width property

Obtiene y establece el ancho de la columna en unidades de caracteres.

```csharp
public double Width { get; set; }
```

### Observaciones

Para la hoja de cálculo, el ancho de columna se mide como el número de caracteres del ancho máximo de dígito de los números 0~9 tal como se renderiza en la fuente del estilo normal.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer el ancho para la columna 3 (índice 2)
            worksheet.Cells.Columns[2].Width = 25.5;
            
            // Establecer el ancho para la columna 4 (índice 3)
            worksheet.Cells.Columns[3].Width = 40.0;
            
            // Obtener y mostrar los anchos
            Console.WriteLine("Column 3 Width: " + worksheet.Cells.Columns[2].Width);
            Console.WriteLine("Column 4 Width: " + worksheet.Cells.Columns[3].Width);
            
            // Guarda el libro de trabajo
            workbook.Save("ColumnWidthDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


