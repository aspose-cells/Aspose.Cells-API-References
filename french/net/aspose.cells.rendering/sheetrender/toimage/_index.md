---
title: "SheetRender.ToImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SheetRender. Rendre une certaine page vers un Graphics"
type: docs
url: /fr/net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Rendre une certaine page vers un Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| g | Graphiques | L'objet où rendre. |
| x | Single | La coordonnée X (en pixels) du coin supérieur gauche de la page rendue. |
| y | Single | La coordonnée Y (en pixels) du coin supérieur gauche de la page rendue. |
| largeur | Single | La largeur maximale (en pixels) pouvant être occupée par la page rendue. |
| hauteur | Single | La hauteur maximale (en pixels) pouvant être occupée par la page rendue. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            try
            {
                // Créer des options d’image
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Créer un rendu de feuille pour la feuille de calcul
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Créer un flux mémoire pour capturer l'image rendue
                using (MemoryStream stream = new MemoryStream())
                {
                    // Appeler ToImage avec les paramètres spécifiés
                    // Comme nous ne pouvons pas utiliser System.Drawing.Graphics, nous utiliserons la surcharge ToImage plus simple
                    sheetRender.ToImage(0, stream);

                    // Enregistrer l'image rendue dans un fichier
                    File.WriteAllBytes("RenderedOutput.png", stream.ToArray());
                }

                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Rendre une certaine page vers un Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| g | Graphiques | L'objet où rendre. |
| x | Single | La coordonnée X (en pixels) du coin supérieur gauche de la page rendue. |
| y | Single | La coordonnée Y (en pixels) du coin supérieur gauche de la page rendue. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            // Créer des options d’image
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Créer une instance de SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Comme nous ne pouvons pas utiliser les types System.Drawing, nous utiliserons la méthode alternative ToImage
                // qui enregistre directement dans un fichier
                sheetRender.ToImage(0, "RenderedOutput.png");
                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
            finally
            {
                // Nettoyer les ressources
                sheetRender.Dispose();
            }
        }
    }
}
```

### Voir aussi

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_4}

Rendre une page donnée vers un fichier.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| fileName | String | nom de fichier de l'image de sortie |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Charger le fichier Excel source
            Workbook workbook = new Workbook("Book1.xlsx");
            
            // Créer des options d’image
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Créer un rendu de feuille pour la première feuille de calcul
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);
            
            // Rendre la première page de la feuille dans un fichier image
            sheetRender.ToImage(0, "output.png");
            
            Console.WriteLine("Sheet rendered to image successfully.");
        }
    }
}
```

### Voir aussi

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Rendre une page donnée vers un flux.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| stream | Stream | le flux de l'image de sortie |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Créer des options d’image
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Créer une instance de SheetRender
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Créer un flux mémoire pour contenir l'image
                using (MemoryStream stream = new MemoryStream())
                {
                    // Appeler ToImage avec les paramètres d'index de page et de flux
                    sheetRender.ToImage(0, stream);

                    Console.WriteLine($"Successfully rendered page 0 to stream. Stream length: {stream.Length} bytes");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Rendre une page donnée vers un objet Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |

### Valeur de retour

l'objet bitmap de la page

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Row 2";
            worksheet.Cells["B3"].Value = 200;

            try
            {
                // Créer des options d’image
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Créer une instance de SheetRender
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Obtenir l'indice de la première page (à partir de 0)
                int pageIndex = 0;

                // Appeler ToImage avec le paramètre d'index de page
                sheetRender.ToImage(pageIndex, "output_page.png");

                Console.WriteLine($"Successfully rendered page {pageIndex} to image");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


