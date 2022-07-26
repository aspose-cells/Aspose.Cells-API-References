---
title: ToImage
second_title: Référence de l'API Aspose.Cells pour .NET
description: Obtient un 32 bitsBitmap objet du graphique.
type: docs
weight: 590
url: /fr/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Obtient un 32 bits`Bitmap` objet du graphique.

```csharp
public Bitmap ToImage()
```

### Return_Value

l'image du tableau.

### Remarques

Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, il renverra null. Veuillez vous référer à[Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.

### Voir également

* class [Chart](../../chart)
* espace de noms [Aspose.Cells.Charts](../../chart)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Obtient un 32 bits`Bitmap` objet du graphique. `ImageOrPrintOptions.ImageFormatImageOrPrintOptions.ImageFormat` , les attributs ImageOrPrintOptions.TiffCompression et ImageOrPrintOptions.Quality sont ignorés.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| options | ImageOrPrintOptions | Options de création d'images supplémentaires |

### Return_Value

l'image du tableau.

### Remarques

Renvoie un objet bitmap 32 bits, de sorte que les attributs ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression et ImageOrPrintOptions.Quality n'affectent pas la méthode. Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, il renverra null. Veuillez vous référer à[Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.

### Exemples

Obtient un objet bitmap avec 200 x dpi et 300 y dpi.

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

### Voir également

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* espace de noms [Aspose.Cells.Charts](../../chart)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image.

```csharp
public void ToImage(string imageFile)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| imageFile | String | Le nom du fichier image avec le chemin complet. |

### Remarques

Le format de l'image est spécifié en utilisant l'extension du nom de fichier. Par exemple, si vous spécifiez "monfichier.png", alors l'image sera enregistrée au format PNG. Les extensions de fichier suivantes sont reconnues : .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien. Veuillez vous référer à[Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.

### Voir également

* class [Chart](../../chart)
* espace de noms [Aspose.Cells.Charts](../../chart)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Crée l'image du graphique et l'enregistre dans un fichier dans le type d'image spécifié.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| imageFile | String | Le nom du fichier image avec le chemin complet. |
| imageType | ImageType | Type d'image dans lequel enregistrer l'image. |

### Remarques

Le type de l'image est spécifié en utilisant`type d'image`. Les types suivants sont pris en charge : ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien. Veuillez vous référer à[Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.

### Voir également

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* espace de noms [Aspose.Cells.Charts](../../chart)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Crée l'image du graphique et l'enregistre dans un fichier au format Jpeg.

```csharp
public void ToImage(string imageFile, long jpegQuality)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| imageFile | String | Le nom du fichier image avec le chemin complet. |
| jpegQuality | Int64 | Qualité Jpeg. |

### Remarques

Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien. Veuillez vous référer à[Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.

### Voir également

* class [Chart](../../chart)
* espace de noms [Aspose.Cells.Charts](../../chart)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Crée l'image du graphique et l'enregistre dans un flux au format Jpeg.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le flux de sortie. |
| jpegQuality | Int64 | Qualité Jpeg. |

### Remarques

Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien. Veuillez vous référer à[Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.

### Voir également

* class [Chart](../../chart)
* espace de noms [Aspose.Cells.Charts](../../chart)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Crée l'image du graphique et l'enregistre dans un flux au format spécifié.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le flux de sortie. |
| imageType | ImageType | Type d'image dans lequel enregistrer l'image. |

### Remarques

Le type de l'image est spécifié en utilisant`type d'image`. Les types suivants sont pris en charge : ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien. Veuillez vous référer[Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.

### Voir également

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* espace de noms [Aspose.Cells.Charts](../../chart)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Crée l'image du graphique et l'enregistre dans un fichier. L'extension du nom de fichier détermine le format de l'image.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| imageFile | String | Le nom du fichier image avec le chemin complet. |
| options | ImageOrPrintOptions | Options de création d'images supplémentaires |

### Remarques

Le format de l'image est spécifié en utilisant l'extension du nom de fichier. Par exemple, si vous spécifiez "monfichier.png", alors l'image sera enregistrée au format PNG. Les extensions de fichier suivantes sont reconnues : .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien. Veuillez vous référer à[Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.

### Exemples

Enregistre au format Tiff avec 300 dpi et compression CCITT4. Enregistre au format Jpeg avec une qualité d'image de 300 dpi et 80.

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
options.TiffCompression = TiffCompression.CompressionCCITT4;

Workbook book = new Workbook(@"test.xls");
book.Worksheets[0].Charts[0].ToImage(@"chart.Tiff", options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions() 
options.HorizontalResolution = 300
options.VerticalResolution = 300
options.TiffCompression = TiffCompression.CompressionCCITT4

Dim book As Workbook =  New Workbook("test.xls")
book.Worksheets(0).Charts(0).ToImage("chart.Tiff", options)

```

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
options.Quality = 80;

Workbook book = new Workbook(@"test.xls");
book.Worksheets[0].Charts[0].ToImage(@"chart.Jpeg", options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions()
options.HorizontalResolution = 300
options.VerticalResolution = 300
options.Quality = 80

Dim book As Workbook =  New Workbook("test.xls")
book.Worksheets(0).Charts(0).ToImage("chart.Jpeg", options)

```

### Voir également

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* espace de noms [Aspose.Cells.Charts](../../chart)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Crée l'image du graphique et l'enregistre dans un flux au format spécifié.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le flux de sortie. |
| options | ImageOrPrintOptions | Options de création d'images supplémentaires |

### Remarques

Le type de l'image est spécifié en utilisant`options.ImageType`. Les formats suivants sont pris en charge : ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien. Veuillez vous référer à[Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.

### Voir également

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* espace de noms [Aspose.Cells.Charts](../../chart)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
