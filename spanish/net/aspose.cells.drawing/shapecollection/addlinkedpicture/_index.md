---
title: "ShapeCollection.AddLinkedPicture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agregar una imagen vinculada"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addlinkedpicture/
---
## ShapeCollection.AddLinkedPicture method

Agrega una imagen vinculada.

```csharp
public Picture AddLinkedPicture(int topRow, int leftColumn, int height, int width, 
    string sourceFullName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| altura | Int32 | La altura de la forma. En unidades de píxeles |
| ancho | Int32 | El ancho de la forma. En unidades de píxeles |
| sourceFullName | String | La ruta y el nombre del archivo fuente para la imagen vinculada |

### Valor de retorno

[`Picture`](../../picture/) Picture object.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLinkedPictureWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar texto de muestra a la celda A1
            worksheet.Cells["A1"].PutValue("Image will be linked below:");
            
            // Agregar imagen vinculada a la hoja de cálculo
            string imageUrl = "https://example.com/sample.jpg";
            worksheet.Shapes.AddLinkedPicture(1, 1, 100, 100, imageUrl);
            
            // Guarda el libro de trabajo
            workbook.Save("output_with_linked_picture.xlsx");
            
            Console.WriteLine("Workbook saved with linked picture.");
        }
    }
}
```

### Ver también

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


