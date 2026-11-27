---
title: "Shape.ToImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Skapar bild av formen och sparar den till en ström i angivet format"
type: docs
url: /sv/net/aspose.cells.drawing/shape/toimage/
---
## ToImage(Stream, ImageType) {#toimage_1}

Skapar formens bild och sparar den till en ström i det angivna formatet.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Utdatastreamen. |
| imageType | ImageType | Typen att spara bilden i. |

### Anmärkningar

Följande format stöds: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Konvertera formen till bildström
            using (MemoryStream imageStream = new MemoryStream())
            {
                shape.ToImage(imageStream, ImageType.Png);
                Console.WriteLine("Shape converted to image stream successfully");
            }
        }
    }
}
```

### Se även

* enum [ImageType](../../imagetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_3}

Sparar formen till en fil.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Ställ in bildalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                HorizontalResolution = 300,
                VerticalResolution = 300
            };

            // Spara formen som bild
            shape.ToImage("shape_image.png", options);
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_2}

Sparar formen till en ström.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

### Exempel

```csharp

[C#]
MemoryStream imageStream = new MemoryStream();
ImageOrPrintOptions op = new ImageOrPrintOptions();
shape.ToImage(imageStream, op);
```

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage}

Returnerar bitmap-objektet för formen.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

### Exempel

```csharp

[C#]
ImageOrPrintOptions op = new ImageOrPrintOptions();
System.Drawing.Bitmap btm = shape.ToImage(op);
```

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


