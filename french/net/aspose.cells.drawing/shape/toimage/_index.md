---
title: "Shape.ToImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Crée l'image de la forme et l'enregistre dans un flux au format spécifié"
type: docs
url: /fr/net/aspose.cells.drawing/shape/toimage/
---
## ToImage(Stream, ImageType) {#toimage_1}

Crée l'image de la forme et l'enregistre dans un flux au format spécifié.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux de sortie. |
| imageType | ImageType | Le type dans lequel enregistrer l'image. |

### Remarques

Les formats suivants sont pris en charge : .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'exemple avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Convertir la forme en flux d'image
            using (MemoryStream imageStream = new MemoryStream())
            {
                shape.ToImage(imageStream, ImageType.Png);
                Console.WriteLine("Shape converted to image stream successfully");
            }
        }
    }
}
```

### Voir aussi

* enum [ImageType](../../imagetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_3}

Enregistre la forme dans un fichier.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'exemple avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Définissez les options d’image
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                HorizontalResolution = 300,
                VerticalResolution = 300
            };

            // Enregistrer la forme en image
            shape.ToImage("shape_image.png", options);
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_2}

Enregistre la forme dans un flux.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

### Exemples

```csharp

[C#]
MemoryStream imageStream = new MemoryStream();
ImageOrPrintOptions op = new ImageOrPrintOptions();
shape.ToImage(imageStream, op);
```

### Voir aussi

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage}

Retourne l'objet bitmap de la forme .

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

### Exemples

```csharp

[C#]
ImageOrPrintOptions op = new ImageOrPrintOptions();
System.Drawing.Bitmap btm = shape.ToImage(op);
```

### Voir aussi

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


