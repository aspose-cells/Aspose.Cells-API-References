---
title: ToImage
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Ottiene un 32 bitBitmap oggetto del grafico.
type: docs
weight: 590
url: /it/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Ottiene un 32 bit`Bitmap` oggetto del grafico.

```csharp
public Bitmap ToImage()
```

### Valore di ritorno

l'immagine del grafico.

### Osservazioni

Se la larghezza o l'altezza è zero o il grafico non è supportato in base all'elenco dei grafici supportati, restituirà null. Fare riferimento a[Elenco dei grafici supportati](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) per maggiori dettagli.

### Guarda anche

* class [Chart](../../chart)
* spazio dei nomi [Aspose.Cells.Charts](../../chart)
* assemblea [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Ottiene un 32 bit`Bitmap` oggetto del grafico. `ImageOrPrintOptions.ImageFormat` , gli attributi ImageOrPrintOptions.TiffCompression e ImageOrPrintOptions.Quality vengono ignorati.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | ImageOrPrintOptions | Opzioni aggiuntive per la creazione di immagini |

### Valore di ritorno

l'immagine del grafico.

### Osservazioni

Restituisce un oggetto bitmap a 32 bit, quindi gli attributi ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression e ImageOrPrintOptions.Quality non influiscono sul metodo. Se la larghezza o l'altezza è zero o il grafico non è supportato in base all'elenco dei grafici supportati, restituirà null. Fare riferimento a[Elenco dei grafici supportati](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) per maggiori dettagli.

### Esempi

Ottiene un oggetto bitmap con 200 x dpi e 300 y dpi.

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

### Guarda anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* spazio dei nomi [Aspose.Cells.Charts](../../chart)
* assemblea [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Crea l'immagine del grafico e la salva in un file. L'estensione del nome del file determina il formato dell'immagine.

```csharp
public void ToImage(string imageFile)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | String | Il nome del file immagine con il percorso completo. |

### Osservazioni

Il formato dell'immagine viene specificato utilizzando l'estensione del nome del file. Ad esempio, se si specifica "myfile.png", l'immagine verrà salvata nel formato PNG. Sono riconosciute le seguenti estensioni di file: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato in base all'elenco dei grafici supportati, questo metodo non avrà effetto. Fare riferimento a[Elenco dei grafici supportati](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) per maggiori dettagli.

### Guarda anche

* class [Chart](../../chart)
* spazio dei nomi [Aspose.Cells.Charts](../../chart)
* assemblea [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Crea l'immagine del grafico e la salva in un file del tipo di immagine specificato.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | String | Il nome del file immagine con il percorso completo. |
| imageType | ImageType | Il tipo di immagine in cui salvare l'immagine. |

### Osservazioni

Il tipo di immagine viene specificato utilizzando`tipo di immagine`. Sono supportati i seguenti tipi: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato in base all'elenco dei grafici supportati, questo metodo non avrà effetto. Fare riferimento a[Elenco dei grafici supportati](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) per maggiori dettagli.

### Guarda anche

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* spazio dei nomi [Aspose.Cells.Charts](../../chart)
* assemblea [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Crea l'immagine del grafico e la salva in un file in formato Jpeg.

```csharp
public void ToImage(string imageFile, long jpegQuality)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | String | Il nome del file immagine con il percorso completo. |
| jpegQuality | Int64 | Qualità JPEG. |

### Osservazioni

Se la larghezza o l'altezza è zero o il grafico non è supportato in base all'elenco dei grafici supportati, questo metodo non avrà effetto. Fare riferimento a[Elenco dei grafici supportati](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) per maggiori dettagli.

### Guarda anche

* class [Chart](../../chart)
* spazio dei nomi [Aspose.Cells.Charts](../../chart)
* assemblea [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Crea l'immagine del grafico e la salva in uno stream nel formato Jpeg.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso di output. |
| jpegQuality | Int64 | Qualità JPEG. |

### Osservazioni

Se la larghezza o l'altezza è zero o il grafico non è supportato in base all'elenco dei grafici supportati, questo metodo non avrà effetto. Fare riferimento a[Elenco dei grafici supportati](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) per maggiori dettagli.

### Guarda anche

* class [Chart](../../chart)
* spazio dei nomi [Aspose.Cells.Charts](../../chart)
* assemblea [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Crea l'immagine del grafico e la salva in un flusso nel formato specificato.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso di output. |
| imageType | ImageType | Il tipo di immagine in cui salvare l'immagine. |

### Osservazioni

Il tipo di immagine viene specificato utilizzando`tipo di immagine`. Sono supportati i seguenti tipi: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato in base all'elenco dei grafici supportati, questo metodo non avrà effetto. Fare riferimento[Elenco dei grafici supportati](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) per maggiori dettagli.

### Guarda anche

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* spazio dei nomi [Aspose.Cells.Charts](../../chart)
* assemblea [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Crea l'immagine del grafico e la salva in un file. L'estensione del nome del file determina il formato dell'immagine.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | String | Il nome del file immagine con il percorso completo. |
| options | ImageOrPrintOptions | Opzioni aggiuntive per la creazione di immagini |

### Osservazioni

Il formato dell'immagine viene specificato utilizzando l'estensione del nome del file. Ad esempio, se si specifica "myfile.png", l'immagine verrà salvata nel formato PNG. Sono riconosciute le seguenti estensioni di file: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato in base all'elenco dei grafici supportati, questo metodo non avrà effetto. Fare riferimento a[Elenco dei grafici supportati](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) per maggiori dettagli.

### Esempi

Salva su Tiff con 300 dpi e compressione CCITT4. Salva in Jpeg con 300 dpi e 80 qualità dell'immagine.

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

### Guarda anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* spazio dei nomi [Aspose.Cells.Charts](../../chart)
* assemblea [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Crea l'immagine del grafico e la salva in un flusso nel formato specificato.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso di output. |
| options | ImageOrPrintOptions | Opzioni aggiuntive per la creazione di immagini |

### Osservazioni

Il tipo di immagine viene specificato utilizzando`opzioni.TipoImmagine`. Sono supportati i seguenti formati: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato in base all'elenco dei grafici supportati, questo metodo non avrà effetto. Fare riferimento a[Elenco dei grafici supportati](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) per maggiori dettagli.

### Guarda anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* spazio dei nomi [Aspose.Cells.Charts](../../chart)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
