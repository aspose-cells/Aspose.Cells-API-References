---
title: ToImage
second_title: Aspose.Cells för .NET API-referens
description: Får en 32-bitarsBitmapp objekt i diagrammet.
type: docs
weight: 590
url: /sv/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Får en 32-bitars`Bitmapp` objekt i diagrammet.

```csharp
public Bitmap ToImage()
```

### Returvärde

bilden av diagrammet.

### Anmärkningar

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer det att returnera null. Se till[Sjökortslista som stöds](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer information.

### Se även

* class [Chart](../../chart)
* namnutrymme [Aspose.Cells.Charts](../../chart)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Får en 32-bitars`Bitmapp` objekt i diagrammet. `ImageOrPrintOptions.ImageFormat` , ImageOrPrintOptions.TiffCompression och ImageOrPrintOptions.Kvalitetsattribut ignoreras.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | ImageOrPrintOptions | Ytterligare bildskapande alternativ |

### Returvärde

bilden av diagrammet.

### Anmärkningar

Returnerar ett 32-bitars bitmappsobjekt, så attributen ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression och ImageOrPrintOptions.Quality påverkar inte metoden. Om attributen noll eller höjd stöds enligt listan eller listan stöds inte enligt diagrammet. returnerar null. Se[Sjökortslista som stöds](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer information.

### Exempel

Får ett bitmappsobjekt med 200 x dpi och 300 y dpi.

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

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* namnutrymme [Aspose.Cells.Charts](../../chart)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Skapar diagrambilden och sparar den i en fil. Filnamnstillägget bestämmer formatet på bilden.

```csharp
public void ToImage(string imageFile)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | String | Bildfilens namn med fullständig sökväg. |

### Anmärkningar

Bildens format specificeras genom att använda filnamnstillägget. Om du till exempel anger "minfil.png", kommer bilden att sparas i PNG-formatet. Följande filtillägg känns igen: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer denna metod inte att göra något. Se till[Sjökortslista som stöds](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer information.

### Se även

* class [Chart](../../chart)
* namnutrymme [Aspose.Cells.Charts](../../chart)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Skapar diagrambilden och sparar den i en fil i angiven bildtyp.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | String | Bildfilens namn med fullständig sökväg. |
| imageType | ImageType | Bildtypen där bilden ska sparas. |

### Anmärkningar

Typen av bilden anges med hjälp av`bildtyp`. Följande typer stöds: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer denna metod inte att göra något. Se till[Sjökortslista som stöds](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer information.

### Se även

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* namnutrymme [Aspose.Cells.Charts](../../chart)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Skapar diagrambilden och sparar den i en fil i Jpeg-format.

```csharp
public void ToImage(string imageFile, long jpegQuality)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | String | Bildfilens namn med fullständig sökväg. |
| jpegQuality | Int64 | Jpeg-kvalitet. |

### Anmärkningar

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer denna metod inte att göra något. Se till[Sjökortslista som stöds](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer information.

### Se även

* class [Chart](../../chart)
* namnutrymme [Aspose.Cells.Charts](../../chart)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Skapar diagrambilden och sparar den i en ström i Jpeg-format.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | Utgångsströmmen. |
| jpegQuality | Int64 | Jpeg-kvalitet. |

### Anmärkningar

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer denna metod inte att göra något. Se till[Sjökortslista som stöds](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer information.

### Se även

* class [Chart](../../chart)
* namnutrymme [Aspose.Cells.Charts](../../chart)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Skapar diagrambilden och sparar den i en ström i angivet format.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | Utgångsströmmen. |
| imageType | ImageType | Bildtypen där bilden ska sparas. |

### Anmärkningar

Typen av bilden anges med hjälp av`bildtyp`. Följande typer stöds: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer den här metoden inte att göra något. Se vänligen[Sjökortslista som stöds](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer information.

### Se även

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* namnutrymme [Aspose.Cells.Charts](../../chart)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Skapar diagrambilden och sparar den i en fil. Filnamnstillägget bestämmer formatet på bilden.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | String | Bildfilens namn med fullständig sökväg. |
| options | ImageOrPrintOptions | Ytterligare bildskapande alternativ |

### Anmärkningar

Bildens format specificeras genom att använda filnamnstillägget. Om du till exempel anger "minfil.png", kommer bilden att sparas i PNG-formatet. Följande filtillägg känns igen: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer denna metod inte att göra något. Se till[Sjökortslista som stöds](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer information.

### Exempel

Sparar till Tiff med 300 dpi och CCITT4-komprimering. Sparar till Jpeg med 300 dpi och 80 bildkvalitet.

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

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* namnutrymme [Aspose.Cells.Charts](../../chart)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Skapar diagrambilden och sparar den i en ström i angivet format.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | Utgångsströmmen. |
| options | ImageOrPrintOptions | Ytterligare bildskapande alternativ |

### Anmärkningar

Typen av bilden anges med hjälp av`options.ImageType`. Följande format stöds: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer denna metod inte att göra något. Se till[Sjökortslista som stöds](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer information.

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* namnutrymme [Aspose.Cells.Charts](../../chart)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
