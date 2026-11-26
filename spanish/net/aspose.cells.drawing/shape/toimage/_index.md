---
title: "Shape.ToImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Crea la imagen de la forma y la guarda en un flujo en el formato especificado"
type: docs
url: /es/net/aspose.cells.drawing/shape/toimage/
---
## ToImage(Stream, ImageType) {#toimage_1}

Crea la imagen de la forma y la guarda en un flujo en el formato especificado.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de salida. |
| imageType | ImageType | El tipo en el que guardar la imagen. |

### Observaciones

Los siguientes formatos son compatibles: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodToImageWithStreamImageTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Convertir la forma a un flujo de imagen
            using (MemoryStream imageStream = new MemoryStream())
            {
                shape.ToImage(imageStream, ImageType.Png);
                Console.WriteLine("Shape converted to image stream successfully");
            }
        }
    }
}
```

### Ver también

* enum [ImageType](../../imagetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_3}

Guarda la forma en un archivo.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ShapeMethodToImageWithStringImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Establezca opciones de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                HorizontalResolution = 300,
                VerticalResolution = 300
            };

            // Guardar la forma como imagen
            shape.ToImage("shape_image.png", options);
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_2}

Guarda la forma en un flujo.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

### Ejemplos

```csharp

[C#]
MemoryStream imageStream = new MemoryStream();
ImageOrPrintOptions op = new ImageOrPrintOptions();
shape.ToImage(imageStream, op);
```

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage}

Devuelve el objeto bitmap de la forma.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

### Ejemplos

```csharp

[C#]
ImageOrPrintOptions op = new ImageOrPrintOptions();
System.Drawing.Bitmap btm = shape.ToImage(op);
```

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


