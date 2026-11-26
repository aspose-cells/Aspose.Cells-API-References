---
title: "ShapeCollection.AddFreeFloatingShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Añade una forma flotante libre a la hoja de cálculo. Solo se aplica a formas de línea/imagen"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addfreefloatingshape/
---
## ShapeCollection.AddFreeFloatingShape method

Agrega una forma flotante libre a la hoja de cálculo.Solo se aplica a la forma de línea/imagen.

```csharp
public Shape AddFreeFloatingShape(MsoDrawingType type, int top, int left, int height, int width, 
    byte[] imageData, bool isOriginalSize)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | MsoDrawingType | El tipo de forma. |
| superior | Int32 | Representa el desplazamiento vertical de la forma desde la fila superior de la hoja de cálculo, en unidades de píxel. |
| izquierda | Int32 | Representa el desplazamiento horizontal de la forma desde la columna izquierda de la hoja de cálculo, en unidades de píxel. |
| altura | Int32 | Representa la altura del LineShape, en unidades de píxel. |
| ancho | Int32 | Representa el ancho del LineShape, en unidades de píxel. |
| imageData | Byte[] | Los datos de imagen, solo se aplican a la foto. |
| isOriginalSize | Booleano | Indica si la forma usa el tamaño original cuando la forma es una imagen. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeFloatingShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar una forma de línea
            Shape floatingShape_Line = shapes.AddFreeFloatingShape(
                MsoDrawingType.Line, 
                100, 100, 100, 50, 
                null, 
                false);

            // Añade una forma de imagen (usando datos de imagen de ejemplo)
            byte[] imageData = null;
            try
            {
                using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
                {
                    imageData = new byte[fs.Length];
                    fs.Read(imageData, 0, (int)fs.Length);
                }
            }
            catch
            {
                // Crea datos de imagen ficticios si no se encuentra el archivo
                imageData = new byte[100];
            }

            Shape floatingShape_Picture = shapes.AddFreeFloatingShape(
                MsoDrawingType.Picture, 
                200, 100, 100, 50, 
                imageData, 
                false);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


