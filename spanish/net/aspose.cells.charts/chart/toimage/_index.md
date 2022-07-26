---
title: ToImage
second_title: Referencia de API de Aspose.Cells para .NET
description: Obtiene una de 32 bitsmapa de bits objeto del gráfico.
type: docs
weight: 590
url: /es/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Obtiene una de 32 bits`mapa de bits` objeto del gráfico.

```csharp
public Bitmap ToImage()
```

### Valor_devuelto

la imagen del gráfico.

### Observaciones

Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, devolverá un valor nulo. Consulte[Lista de gráficos admitidos](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) para más detalles.

### Ver también

* class [Chart](../../chart)
* espacio de nombres [Aspose.Cells.Charts](../../chart)
* asamblea [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Obtiene una de 32 bits`mapa de bits` objeto del gráfico. `ImageOrPrintOptions.ImageFormat` , los atributos ImageOrPrintOptions.TiffCompression e ImageOrPrintOptions.Quality se ignoran.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| options | ImageOrPrintOptions | Opciones adicionales de creación de imágenes |

### Valor_devuelto

la imagen del gráfico.

### Observaciones

Devuelve un objeto de mapa de bits de 32 bits, por lo que los atributos ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression e ImageOrPrintOptions.Quality no afectan al método. devolverá null. Consulte[Lista de gráficos admitidos](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) para más detalles.

### Ejemplos

Obtiene un objeto bitmap con 200 x dpi y 300 y dpi.

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

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* espacio de nombres [Aspose.Cells.Charts](../../chart)
* asamblea [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Crea la imagen del gráfico y la guarda en un archivo. La extensión del nombre del archivo determina el formato de la imagen.

```csharp
public void ToImage(string imageFile)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| imageFile | String | El nombre del archivo de imagen con la ruta completa. |

### Observaciones

El formato de la imagen se especifica utilizando la extensión del nombre de archivo. Por ejemplo, si especifica "miarchivo.png", la imagen se guardará en formato PNG. Se reconocen las siguientes extensiones de archivo: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada. Consulte[Lista de gráficos admitidos](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) para más detalles.

### Ver también

* class [Chart](../../chart)
* espacio de nombres [Aspose.Cells.Charts](../../chart)
* asamblea [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Crea la imagen del gráfico y la guarda en un archivo con el tipo de imagen especificado.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| imageFile | String | El nombre del archivo de imagen con la ruta completa. |
| imageType | ImageType | El tipo de imagen en el que guardar la imagen. |

### Observaciones

El tipo de la imagen se especifica usando`tipo de imagen`. Se admiten los siguientes tipos: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada. Consulte[Lista de gráficos admitidos](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) para más detalles.

### Ver también

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* espacio de nombres [Aspose.Cells.Charts](../../chart)
* asamblea [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Crea la imagen del gráfico y la guarda en un archivo en formato Jpeg.

```csharp
public void ToImage(string imageFile, long jpegQuality)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| imageFile | String | El nombre del archivo de imagen con la ruta completa. |
| jpegQuality | Int64 | Calidad JPEG. |

### Observaciones

Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada. Consulte[Lista de gráficos admitidos](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) para más detalles.

### Ver también

* class [Chart](../../chart)
* espacio de nombres [Aspose.Cells.Charts](../../chart)
* asamblea [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Crea la imagen del gráfico y la guarda en una secuencia en formato Jpeg.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de salida. |
| jpegQuality | Int64 | Calidad JPEG. |

### Observaciones

Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada. Consulte[Lista de gráficos admitidos](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) para más detalles.

### Ver también

* class [Chart](../../chart)
* espacio de nombres [Aspose.Cells.Charts](../../chart)
* asamblea [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Crea la imagen del gráfico y la guarda en una secuencia en el formato especificado.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de salida. |
| imageType | ImageType | El tipo de imagen en el que guardar la imagen. |

### Observaciones

El tipo de la imagen se especifica usando`tipo de imagen`. Se admiten los siguientes tipos: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada. Consulte[Lista de gráficos admitidos](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) para más detalles.

### Ver también

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* espacio de nombres [Aspose.Cells.Charts](../../chart)
* asamblea [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Crea la imagen del gráfico y la guarda en un archivo. La extensión del nombre del archivo determina el formato de la imagen.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| imageFile | String | El nombre del archivo de imagen con la ruta completa. |
| options | ImageOrPrintOptions | Opciones adicionales de creación de imágenes |

### Observaciones

El formato de la imagen se especifica utilizando la extensión del nombre de archivo. Por ejemplo, si especifica "miarchivo.png", la imagen se guardará en formato PNG. Se reconocen las siguientes extensiones de archivo: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada. Consulte[Lista de gráficos admitidos](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) para más detalles.

### Ejemplos

Guarda en Tiff con 300 dpi y compresión CCITT4. Guarda en JPEG con 300 ppp y calidad de imagen 80.

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

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* espacio de nombres [Aspose.Cells.Charts](../../chart)
* asamblea [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Crea la imagen del gráfico y la guarda en una secuencia en el formato especificado.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de salida. |
| options | ImageOrPrintOptions | Opciones adicionales de creación de imágenes |

### Observaciones

El tipo de la imagen se especifica usando`opciones.ImageType`. Se admiten los siguientes formatos: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada. Consulte[Lista de gráficos admitidos](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) para más detalles.

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* espacio de nombres [Aspose.Cells.Charts](../../chart)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
