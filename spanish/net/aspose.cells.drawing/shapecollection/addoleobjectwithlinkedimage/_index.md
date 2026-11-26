---
title: "ShapeCollection.AddOleObjectWithLinkedImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agregar una imagen vinculada"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addoleobjectwithlinkedimage/
---
## ShapeCollection.AddOleObjectWithLinkedImage method

Agrega una imagen vinculada.

```csharp
public OleObject AddOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, 
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddOleObjectWithLinkedImageWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ruta al archivo de imagen que se vinculará
            string imagePath = "example.jpg";

            try
            {
                // Llame al método AddOleObjectWithLinkedImage con parámetros específicos
                OleObject oleObject = worksheet.Shapes.AddOleObjectWithLinkedImage(
                    1,  // upperLeftRow
                    1,  // upperLeftColumn
                    200, // height
                    300, // width
                    imagePath); // sourceFullName

                // Establezca propiedades adicionales para el OleObject
                oleObject.DisplayAsIcon = false;
                oleObject.IsAutoSize = true;

                Console.WriteLine("OLE object with linked image added successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddOleObjectWithLinkedImage method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("AddOleObjectWithLinkedImageDemo.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


