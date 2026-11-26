---
title: "ShapeCollection.AddPicture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega una imagen a la colección"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addpicture/
---
## AddPicture(int, int, int, int, Stream) {#addpicture}

Agrega una picture a la colección.

```csharp
public Picture AddPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| bottomRow | Int32 | Índice de fila inferior derecha |
| rightColumn | Int32 | Índice de columna inferior derecha |
| stream | Stream | Objeto Stream que contiene los datos de la imagen. |

### Valor de retorno

[`Picture`](../../picture/) Picture object.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddPictureWithInt32Int32Int32Int32StreamDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar una imagen desde un flujo de archivo
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                Picture picture = shapes.AddPicture(1, 0, 1, 0, fs);
            }

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddPicture(int, int, Stream, int, int) {#addpicture_1}

Agrega una picture a la colección.

```csharp
public Picture AddPicture(int topRow, int leftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| stream | Stream | Objeto Stream que contiene los datos de la imagen. |
| widthScale | Int32 | Escala del ancho de la imagen, un porcentaje. |
| heightScale | Int32 | Escala de la altura de la imagen, un porcentaje. |

### Valor de retorno

[`Picture`](../../picture/) Picture object.

### Ejemplos

```csharp

[C#]
//agregar una picture
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    Picture picture = shapes.AddPicture(1, 1, fs, 50, 60);
}
```

### Ver también

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


