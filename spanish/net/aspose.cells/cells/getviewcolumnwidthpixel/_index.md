---
title: "Cells.GetViewColumnWidthPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el ancho en diferentes tipos de vista"
type: docs
url: /es/net/aspose.cells/cells/getviewcolumnwidthpixel/
---
## Cells.GetViewColumnWidthPixel method

Obtiene el ancho en diferentes tipos de vista.

```csharp
public int GetViewColumnWidthPixel(int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | El índice de columna. |

### Valor de retorno

el ancho de la columna en unidades de píxeles

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer el tipo de vista a PageLayoutView
            worksheet.ViewType = ViewType.PageLayoutView;
            
            // Establecer el ancho de la columna en caracteres (se convertirá a píxeles)
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Obtener el ancho de la columna en píxeles
            int columnWidthInPixels = worksheet.Cells.GetViewColumnWidthPixel(0);
            
            // Mostrar el resultado
            Console.WriteLine("Column width in pixels: " + columnWidthInPixels);
            
            // Guarda el libro de trabajo
            workbook.Save("ColumnWidthTest.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


