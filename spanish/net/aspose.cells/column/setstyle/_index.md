---
title: "Column.SetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Column. Establece el estilo de esta columna"
type: docs
url: /es/net/aspose.cells/column/setstyle/
---
## Column.SetStyle method

Establece el estilo de esta columna.

```csharp
public void SetStyle(Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | el estilo que se usará como estilo predeterminado para las celdas en esta columna. |

### Observaciones

Este método solo establece el estilo dado como estilo predeterminado para esta columna, sin cambiar la configuración de estilo de las celdas existentes en esta columna. Para actualizar la configuración de estilo de las celdas existentes al estilo especificado al mismo tiempo, por favor use [`ApplyStyle`](../applystyle/)

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnMethodSetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la primera columna
            Column column = worksheet.Cells.Columns[0];

            // Crear un nuevo estilo desde el libro de trabajo
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            try
            {
                // Aplicar el estilo personalizado a toda la columna
                column.SetStyle(style);
                
                Console.WriteLine($"Style applied successfully to column {column.Index}");
                Console.WriteLine($"Font: {style.Font.Name}, Size: {style.Font.Size}, Bold: {style.Font.IsBold}");
                Console.WriteLine($"Background: {style.ForegroundColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStyle method: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("ColumnMethodSetStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


