---
title: "Chart.ToImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Chart. Obtient un objet Bitmap 32 bits du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Obtient un objet `Bitmap` 32 bits du graphique.

```csharp
public Bitmap ToImage()
```

### Valeur de retour

l'image du graphique.

### Remarques

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, il renverra null.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["B4"].PutValue(1500);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);
            
            // Convertir le graphique en image et l'enregistrer dans un fichier
            chart.ToImage("ChartImage.png", ImageType.Png);
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Obtient un objet `Bitmap` 32 bits du graphique. Les attributs `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression et ImageOrPrintOptions.Quality sont ignorés.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | Options supplémentaires de création d'image |

### Valeur de retour

l'image du graphique.

### Remarques

Renvoie un objet bitmap 32 bits, de sorte que les attributs ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression et ImageOrPrintOptions.Quality n'affectent pas la méthode. Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, il renverra null.

### Exemples

Obtient un objet bitmap avec 200 dpi en x et 300 dpi en y.

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 200;
options.VerticalResolution = 300;

Workbook book = new Workbook(@"test.xls");
Bitmap chartObject = book.Worksheets[0].Charts[0].ToImage(options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions() 
options.HorizontalResolution = 200
options.VerticalResolution = 300

Dim book As Workbook =  New Workbook("test.xls")
Dim chartObject As Bitmap = book.Worksheets(0).Charts(0).ToImage(options)

```

### Voir aussi

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image.

```csharp
public void ToImage(string imageFile)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| imageFile | String | Le nom du fichier image avec le chemin complet. |

### Remarques

Le format de l'image est spécifié en utilisant l'extension du nom de fichier. Par exemple, si vous spécifiez "myfile.png", l'image sera enregistrée au format PNG. Les extensions de fichier suivantes sont reconnues : .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(45);
            worksheet.Cells["B3"].PutValue(55);
            
            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Enregistrer le graphique en tant qu'image
            chart.ToImage("ChartImage.jpg");
            
            Console.WriteLine("Chart saved as image successfully.");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageFormat) {#toimage_10}

Crée l'image du graphique et l'enregistre dans un fichier au format spécifié.

```csharp
[Obsolete("Use Chart.ToImage(string, ImageType) method instead.")]
public void ToImage(string imageFile, ImageFormat imageFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| imageFile | String | Le nom du fichier image avec le chemin complet. |
| imageFormat | ImageFormat | Le format dans lequel enregistrer l'image. |

### Remarques

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la méthode Chart.ToImage(string, ImageType). Cette propriété sera supprimée 12 mois plus tard à compter de juillet 2022. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Crée l'image du graphique et l'enregistre dans un fichier au type d'image spécifié.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| imageFile | String | Le nom du fichier image avec le chemin complet. |
| imageType | ImageType | Le type d'image dans lequel enregistrer l'image. |

### Remarques

Le type de l'image est spécifié en utilisant `imageType`. Les types suivants sont pris en charge : ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringImageTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(7);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Enregistrer le graphique en image avec le ImageType spécifié
            chart.ToImage("output_chart.png", ImageType.Png);

            Console.WriteLine("Chart saved to image successfully.");
        }
    }
}
```

### Voir aussi

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Crée l'image du graphique et l'enregistre dans un fichier au format Jpeg.

```csharp
[Obsolete("Use Chart.ToImage(string,ImageOrPrintOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ToImage(string imageFile, long jpegQuality)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| imageFile | String | Le nom du fichier image avec le chemin complet. |
| jpegQuality | Int64 | Qualité Jpeg. |

### Remarques

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien. NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode ToImage(string,ImageOrPrintOptions) avec la qualité spécifiée. Cette méthode sera supprimée 12 mois plus tard, à compter de mars 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodToImageWithStringInt64Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);
            
            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            try
            {
                // Appelez la méthode ToImage avec les paramètres (String, Int64)
                string imagePath = "ChartImage.jpg";
                long jpegQuality = 90; // Quality percentage (0-100)
                chart.ToImage(imagePath, jpegQuality);
                
                Console.WriteLine($"Chart saved as image successfully to: {imagePath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToImage method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("ChartToImageDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Crée l'image du graphique et l'enregistre dans un flux au format Jpeg.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux de sortie. |
| jpegQuality | Int64 | Qualité Jpeg. |

### Remarques

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamInt64Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Créer un flux mémoire pour enregistrer l'image
                using (MemoryStream stream = new MemoryStream())
                {
                    // Appelez la méthode ToImage avec les paramètres Stream et Int64.
                    // La qualité JPEG est spécifiée à 80 (la plage valide est généralement de 0 à 100).
                    chart.ToImage(stream, 80);

                    // Afficher le message de succès
                    Console.WriteLine("Chart successfully converted to image with JPEG quality 80");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Enregistrez le classeur
                    workbook.Save("ChartToImageDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageFormat) {#toimage_5}

Crée l'image du graphique et l'enregistre dans un flux au format spécifié.

```csharp
[Obsolete("Use Chart.ToImage(Stream, ImageType) method instead.")]
public void ToImage(Stream stream, ImageFormat imageFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux de sortie. |
| imageFormat | ImageFormat | Le format dans lequel enregistrer l'image. |

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Chart.ToImage(Stream, ImageType). Cette propriété sera supprimée 12 mois plus tard, à compter de juillet 2022. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Créer un flux mémoire pour enregistrer l'image
                using (MemoryStream stream = new MemoryStream())
                {
                    // Appelez la méthode ToImage avec les paramètres Stream et ImageFormat.
                    // Utilisation de Aspose.Cells.Drawing.ImageType à la place de System.Drawing.Imaging.ImageFormat.
                    chart.ToImage(stream, Aspose.Cells.Drawing.ImageType.Png);

                    // Afficher le message de succès
                    Console.WriteLine("Chart successfully saved to stream in PNG format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // En option, enregistrez le flux dans un fichier pour vérification.
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToImage: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Crée l'image du graphique et l'enregistre dans un flux au format spécifié.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux de sortie. |
| imageType | ImageType | Le type d'image dans lequel enregistrer l'image. |

### Remarques

Le type de l'image est spécifié en utilisant `imageType`. Les types suivants sont pris en charge : ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Créer un flux mémoire pour enregistrer l'image
                using (MemoryStream stream = new MemoryStream())
                {
                    // Appelez la méthode ToImage avec les paramètres Stream et ImageType.
                    chart.ToImage(stream, ImageType.Png);

                    // Afficher le message de succès
                    Console.WriteLine("Chart successfully converted to image in PNG format");

                    // Enregistrez l'image dans un fichier à des fins de démonstration.
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
                }

                // Enregistrez le classeur
                workbook.Save("ChartToImageDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| imageFile | String | Le nom du fichier image avec le chemin complet. |
| options | ImageOrPrintOptions | Options supplémentaires de création d'image |

### Remarques

Le format de l'image est spécifié en utilisant l'extension du nom de fichier. Par exemple, si vous spécifiez "myfile.png", l'image sera enregistrée au format PNG. Les extensions de fichier suivantes sont reconnues : .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien. Veuillez consulter la [Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Créer des options d’image
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            options.TiffCompression = TiffCompression.CompressionCCITT4;

            // Chargez le classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple et créer un graphique
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Enregistrer le graphique en image.
            chart.ToImage("chart.tiff", options);
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Crée l'image du graphique et l'enregistre dans un flux au format spécifié.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux de sortie. |
| options | ImageOrPrintOptions | Options supplémentaires de création d'image |

### Remarques

Le type de l'image est spécifié en utilisant `options.ImageType`. Les formats suivants sont pris en charge : ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si la largeur ou la hauteur est zéro ou si le graphique n'est pas pris en charge selon la Liste des graphiques pris en charge, cette méthode ne fera rien. Veuillez consulter la [Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageOrPrintOptDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Créer un flux mémoire pour enregistrer l'image
                using (MemoryStream stream = new MemoryStream())
                {
                    // Créez ImageOrPrintOptions avec des paramètres spécifiques.
                    ImageOrPrintOptions options = new ImageOrPrintOptions();
                    options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                    options.HorizontalResolution = 300;
                    options.VerticalResolution = 300;

                    // Appelez la méthode ToImage avec les paramètres Stream et ImageOrPrintOptions.
                    chart.ToImage(stream, options);

                    // Afficher le message de succès
                    Console.WriteLine("Chart successfully converted to image with custom options");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Enregistrez le classeur
                    workbook.Save("ChartToImageDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


