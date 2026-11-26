---
title: "PictureCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PictureCollection. Añade una imagen a la colección"
type: docs
url: /es/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Agrega una picture a la colección.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| bottomRow | Int32 | Índice de fila inferior derecha |
| rightColumn | Int32 | Índice de columna inferior derecha |
| stream | Stream | Objeto Stream que contiene los datos de la imagen. |

### Valor de retorno

[`Picture`](../../picture/) object index.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32Int32Int32StreamDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añadir una imagen desde el flujo
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(10, 10, 200, 200, fs);
            }

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Agrega una picture a la colección.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, string fileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| bottomRow | Int32 | Índice de fila inferior derecha |
| rightColumn | Int32 | Índice de columna inferior derecha |
| fileName | String | Nombre de archivo de Image. |

### Valor de retorno

[`Picture`](../../picture/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, 5, 5, "image.jpg");

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Agrega una picture a la colección.

```csharp
public int Add(int topRow, int leftColumn, Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| stream | Stream | Objeto Stream que contiene los datos de la imagen. |

### Valor de retorno

[`Picture`](../../picture/) object index.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StreamDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añadir una imagen desde el flujo
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(1, 1, fs);
            }

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Agrega una picture a la colección.

```csharp
public int Add(int topRow, int leftColumn, string fileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| fileName | String | Nombre de archivo de Image. |

### Valor de retorno

[`Picture`](../../picture/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, "image.jpg");

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Agrega una picture a la colección.

```csharp
public int Add(int topRow, int leftColumn, Stream stream, int widthScale, int heightScale)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| stream | Stream | Objeto Stream que contiene los datos de la imagen. |
| widthScale | Int32 | Escala del ancho de la imagen, un porcentaje. |
| heightScale | Int32 | Escala de la altura de la imagen, un porcentaje. |

### Valor de retorno

[`Picture`](../../picture/) object index.

### Ejemplos

```csharp

[C#]
//agregar una picture
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### Ver también

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Agrega una picture a la colección.

```csharp
public int Add(int topRow, int leftColumn, string fileName, int widthScale, int heightScale)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| fileName | String | Nombre de archivo de Image. |
| widthScale | Int32 | Escala del ancho de la imagen, un porcentaje. |
| heightScale | Int32 | Escala de la altura de la imagen, un porcentaje. |

### Valor de retorno

[`Picture`](../../picture/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, "image.jpg", 50, 50);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


