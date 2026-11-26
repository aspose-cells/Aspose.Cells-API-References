---
title: "BorderCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BorderCollection. Obtiene el elemento Border en el índice especificado"
type: docs
url: /es/net/aspose.cells/bordercollection/item/
---
## BorderCollection indexer

Obtiene el elemento [`Border`](../../border/) en el índice especificado.

```csharp
public Border this[BorderType borderType] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| borderType | El borde a recuperar. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class BorderCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Obtener la celda y su estilo
                Cell cell = worksheet.Cells["A1"];
                Style style = cell.GetStyle();

                // Acceder a BorderCollection desde el estilo
                BorderCollection borders = style.Borders;

                // Mostrar el valor actual de la propiedad Item (operación de lectura)
                // Nota: La propiedad Item es de solo lectura y devuelve un objeto Border
                // La propiedad Item requiere un parámetro BorderType
                Border border = borders[BorderType.LeftBorder];
                Console.WriteLine("Border type: " + border.LineStyle);
                Console.WriteLine("Border color: " + border.Color);

                // Guardar el resultado
                workbook.Save("ItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Border](../../border/)
* enum [BorderType](../../bordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


