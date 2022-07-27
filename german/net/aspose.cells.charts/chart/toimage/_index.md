---
title: ToImage
second_title: Aspose.Cells für .NET-API-Referenz
description: Ruft eine 32-Bit-Version abBitmap Objekt des Diagramms.
type: docs
weight: 590
url: /de/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Ruft eine 32-Bit-Version ab`Bitmap` Objekt des Diagramms.

```csharp
public Bitmap ToImage()
```

### Rückgabewert

das Bild des Diagramms.

### Bemerkungen

Wenn die Breite oder Höhe Null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird null zurückgegeben. Siehe bitte[Liste der unterstützten Diagramme](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) für weitere Details.

### Siehe auch

* class [Chart](../../chart)
* namensraum [Aspose.Cells.Charts](../../chart)
* Montage [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Ruft eine 32-Bit-Version ab`Bitmap` Objekt des Diagramms. `ImageOrPrintOptions.ImageFormat` , ImageOrPrintOptions.TiffCompression und ImageOrPrintOptions.Quality werden ignoriert.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | ImageOrPrintOptions | Zusätzliche Bilderzeugungsoptionen |

### Rückgabewert

das Bild des Diagramms.

### Bemerkungen

Gibt ein 32-Bit-Bitmap-Objekt zurück, sodass die Attribute „ImageOrPrintOptions.ImageFormat“, „ImageOrPrintOptions.TiffCompression“ und „ImageOrPrintOptions.Quality “ die Methode nicht beeinflussen gibt null zurück. Siehe bitte[Liste der unterstützten Diagramme](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) für weitere Details.

### Beispiele

Ruft ein Bitmap-Objekt mit 200 x dpi und 300 y dpi ab.

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

### Siehe auch

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* namensraum [Aspose.Cells.Charts](../../chart)
* Montage [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Erstellt das Diagrammbild und speichert es in einer Datei. Die Erweiterung des Dateinamens bestimmt das Format des Bildes.

```csharp
public void ToImage(string imageFile)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | String | Der Bilddateiname mit vollständigem Pfad. |

### Bemerkungen

Das Format des Bildes wird durch die Erweiterung des Dateinamens angegeben. Wenn Sie beispielsweise "myfile.png" angeben, wird das Bild im PNG-Format gespeichert. Folgende Dateierweiterungen werden erkannt: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Wenn die Breite oder Höhe null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken. Bitte beziehen Sie sich auf[Liste der unterstützten Diagramme](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) für weitere Details.

### Siehe auch

* class [Chart](../../chart)
* namensraum [Aspose.Cells.Charts](../../chart)
* Montage [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Bildtyp.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | String | Der Bilddateiname mit vollständigem Pfad. |
| imageType | ImageType | Der Bildtyp, in dem das Bild gespeichert werden soll. |

### Bemerkungen

Der Typ des Bildes wird durch Verwendung angegeben`Bildtyp`. Die folgenden Typen werden unterstützt: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Wenn die Breite oder Höhe null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken. Bitte beziehen Sie sich auf[Liste der unterstützten Diagramme](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) für weitere Details.

### Siehe auch

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* namensraum [Aspose.Cells.Charts](../../chart)
* Montage [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Erstellt das Diagrammbild und speichert es in einer Datei im JPEG-Format.

```csharp
public void ToImage(string imageFile, long jpegQuality)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | String | Der Bilddateiname mit vollständigem Pfad. |
| jpegQuality | Int64 | JPEG-Qualität. |

### Bemerkungen

Wenn die Breite oder Höhe null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken. Bitte beziehen Sie sich auf[Liste der unterstützten Diagramme](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) für weitere Details.

### Siehe auch

* class [Chart](../../chart)
* namensraum [Aspose.Cells.Charts](../../chart)
* Montage [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Erstellt das Diagrammbild und speichert es in einem Stream im JPEG-Format.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Ausgangsstrom. |
| jpegQuality | Int64 | JPEG-Qualität. |

### Bemerkungen

Wenn die Breite oder Höhe null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken. Bitte beziehen Sie sich auf[Liste der unterstützten Diagramme](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) für weitere Details.

### Siehe auch

* class [Chart](../../chart)
* namensraum [Aspose.Cells.Charts](../../chart)
* Montage [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Erstellt das Diagrammbild und speichert es in einem Stream im angegebenen Format.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Ausgangsstrom. |
| imageType | ImageType | Der Bildtyp, in dem das Bild gespeichert werden soll. |

### Bemerkungen

Der Typ des Bildes wird durch Verwendung angegeben`Bildtyp`. Die folgenden Typen werden unterstützt: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Wenn die Breite oder Höhe Null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken. Siehe bitte[Liste der unterstützten Diagramme](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) für weitere Details.

### Siehe auch

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* namensraum [Aspose.Cells.Charts](../../chart)
* Montage [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Erstellt das Diagrammbild und speichert es in einer Datei. Die Erweiterung des Dateinamens bestimmt das Format des Bildes.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | String | Der Bilddateiname mit vollständigem Pfad. |
| options | ImageOrPrintOptions | Zusätzliche Bilderzeugungsoptionen |

### Bemerkungen

Das Format des Bildes wird durch die Erweiterung des Dateinamens angegeben. Wenn Sie beispielsweise "myfile.png" angeben, wird das Bild im PNG-Format gespeichert. Folgende Dateierweiterungen werden erkannt: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Wenn die Breite oder Höhe null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken. Bitte beziehen Sie sich auf[Liste der unterstützten Diagramme](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) für weitere Details.

### Beispiele

Speichert im TIFF-Format mit 300 dpi und CCITT4-Komprimierung. Speichert als JPEG mit 300 dpi und 80 Bildqualität.

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

### Siehe auch

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* namensraum [Aspose.Cells.Charts](../../chart)
* Montage [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Erstellt das Diagrammbild und speichert es in einem Stream im angegebenen Format.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Ausgangsstrom. |
| options | ImageOrPrintOptions | Zusätzliche Bilderzeugungsoptionen |

### Bemerkungen

Der Typ des Bildes wird durch Verwendung angegeben`options.ImageType`. Die folgenden Formate werden unterstützt: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Wenn die Breite oder Höhe null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken. Bitte beziehen Sie sich auf[Liste der unterstützten Diagramme](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) für weitere Details.

### Siehe auch

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* namensraum [Aspose.Cells.Charts](../../chart)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
