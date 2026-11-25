---
title: "Chart.ToImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Ottiene un oggetto Bitmap a 32 bit del grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Ottiene un oggetto `Bitmap` a 32 bit del grafico.

```csharp
public Bitmap ToImage()
```

### Valore di ritorno

l'immagine del grafico.

### Osservazioni

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, restituirà null.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["B4"].PutValue(1500);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);
            
            // Converti il grafico in immagine e salva su file
            chart.ToImage("ChartImage.png", ImageType.Png);
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Ottiene un oggetto `Bitmap` a 32 bit del grafico. Gli attributi `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression e ImageOrPrintOptions.Quality sono ignorati.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | ImageOrPrintOptions | Opzioni aggiuntive per la creazione dell'immagine |

### Valore di ritorno

l'immagine del grafico.

### Osservazioni

Restituisce un oggetto bitmap a 32 bit, quindi gli attributi ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression e ImageOrPrintOptions.Quality non influenzano il metodo. Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, restituirà null.

### Esempi

Ottiene un oggetto bitmap con 200 dpi in x e 300 dpi in y.

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

### Vedi anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Crea l'immagine del grafico e la salva in un file. L'estensione del nome file determina il formato dell'immagine.

```csharp
public void ToImage(string imageFile)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | String | Il nome del file immagine con percorso completo. |

### Osservazioni

Il formato dell'immagine è specificato utilizzando l'estensione del nome file. Ad esempio, se specifichi "myfile.png", l'immagine verrà salvata in formato PNG. Sono riconosciute le seguenti estensioni file: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(45);
            worksheet.Cells["B3"].PutValue(55);
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Salva il grafico come immagine
            chart.ToImage("ChartImage.jpg");
            
            Console.WriteLine("Chart saved as image successfully.");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageFormat) {#toimage_10}

Crea l'immagine del grafico e la salva su un file nel formato specificato.

```csharp
[Obsolete("Use Chart.ToImage(string, ImageType) method instead.")]
public void ToImage(string imageFile, ImageFormat imageFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | String | Il nome del file immagine con percorso completo. |
| imageFormat | ImageFormat | Il formato in cui salvare l'immagine. |

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, utilizza il metodo Chart.ToImage(string, ImageType). Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Crea l'immagine del grafico e la salva in un file nel tipo di immagine specificato.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | String | Il nome del file immagine con percorso completo. |
| imageType | ImageType | Il tipo di immagine in cui salvare l'immagine. |

### Osservazioni

Il tipo di immagine è specificato utilizzando `imageType`. Sono supportati i seguenti tipi: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(7);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Salva il grafico in immagine con ImageType specificato
            chart.ToImage("output_chart.png", ImageType.Png);

            Console.WriteLine("Chart saved to image successfully.");
        }
    }
}
```

### Vedi anche

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Crea l'immagine del grafico e la salva in un file nel formato Jpeg.

```csharp
[Obsolete("Use Chart.ToImage(string,ImageOrPrintOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ToImage(string imageFile, long jpegQuality)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | String | Il nome del file immagine con percorso completo. |
| jpegQuality | Int64 | Qualità Jpeg. |

### Osservazioni

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla. NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo ToImage(string,ImageOrPrintOptions) con la qualità specificata. Questo metodo sarà rimosso 12 mesi dopo, a partire da marzo 2025. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            try
            {
                // Chiama il metodo ToImage con i parametri (String, Int64)
                string imagePath = "ChartImage.jpg";
                long jpegQuality = 90; // Quality percentage (0-100)
                chart.ToImage(imagePath, jpegQuality);
                
                Console.WriteLine($"Chart saved as image successfully to: {imagePath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToImage method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ChartToImageDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Crea l'immagine del grafico e la salva in uno stream nel formato Jpeg.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso di output. |
| jpegQuality | Int64 | Qualità Jpeg. |

### Osservazioni

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Crea un flusso di memoria per salvare l'immagine
                using (MemoryStream stream = new MemoryStream())
                {
                    // Chiama il metodo ToImage con i parametri Stream e Int64
                    // La qualità JPEG è specificata come 80 (l'intervallo valido è tipicamente 0-100)
                    chart.ToImage(stream, 80);

                    // Visualizza il messaggio di successo
                    Console.WriteLine("Chart successfully converted to image with JPEG quality 80");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Salva la cartella di lavoro
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

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageFormat) {#toimage_5}

Crea l'immagine del grafico e la salva in uno stream nel formato specificato.

```csharp
[Obsolete("Use Chart.ToImage(Stream, ImageType) method instead.")]
public void ToImage(Stream stream, ImageFormat imageFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso di output. |
| imageFormat | ImageFormat | Il formato in cui salvare l'immagine. |

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Chart.ToImage(Stream, ImageType). Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2022. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Crea un flusso di memoria per salvare l'immagine
                using (MemoryStream stream = new MemoryStream())
                {
                    // Chiama il metodo ToImage con i parametri Stream e ImageFormat
                    // Utilizzando Aspose.Cells.Drawing.ImageType invece di System.Drawing.Imaging.ImageFormat
                    chart.ToImage(stream, Aspose.Cells.Drawing.ImageType.Png);

                    // Visualizza il messaggio di successo
                    Console.WriteLine("Chart successfully saved to stream in PNG format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // Facoltativamente salva il flusso in un file per verifica
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

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Crea l'immagine del grafico e la salva in uno stream nel formato specificato.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso di output. |
| imageType | ImageType | Il tipo di immagine in cui salvare l'immagine. |

### Osservazioni

Il tipo di immagine è specificato utilizzando `imageType`. Sono supportati i seguenti tipi: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Crea un flusso di memoria per salvare l'immagine
                using (MemoryStream stream = new MemoryStream())
                {
                    // Chiama il metodo ToImage con i parametri Stream e ImageType
                    chart.ToImage(stream, ImageType.Png);

                    // Visualizza il messaggio di successo
                    Console.WriteLine("Chart successfully converted to image in PNG format");

                    // Salva l'immagine in un file per dimostrazione
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
                }

                // Salva la cartella di lavoro
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

### Vedi anche

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Crea l'immagine del grafico e la salva in un file. L'estensione del nome file determina il formato dell'immagine.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | String | Il nome del file immagine con percorso completo. |
| opzioni | ImageOrPrintOptions | Opzioni aggiuntive per la creazione dell'immagine |

### Osservazioni

Il formato dell'immagine è specificato utilizzando l'estensione del nome file. Ad esempio, se specifichi "myfile.png", l'immagine verrà salvata in formato PNG. Sono riconosciute le seguenti estensioni file: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla. Si prega di fare riferimento a [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) per ulteriori dettagli.

### Esempi

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
            // Crea opzioni immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            options.TiffCompression = TiffCompression.CompressionCCITT4;

            // Carica la cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e crea un grafico
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

            // Salva il grafico in immagine
            chart.ToImage("chart.tiff", options);
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Crea l'immagine del grafico e la salva in uno stream nel formato specificato.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso di output. |
| opzioni | ImageOrPrintOptions | Opzioni aggiuntive per la creazione dell'immagine |

### Osservazioni

Il tipo di immagine è specificato usando `options.ImageType`. I seguenti formati sono supportati: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla. Si prega di fare riferimento a [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) per ulteriori dettagli.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Crea un flusso di memoria per salvare l'immagine
                using (MemoryStream stream = new MemoryStream())
                {
                    // Crea ImageOrPrintOptions con impostazioni specifiche
                    ImageOrPrintOptions options = new ImageOrPrintOptions();
                    options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                    options.HorizontalResolution = 300;
                    options.VerticalResolution = 300;

                    // Chiama il metodo ToImage con i parametri Stream e ImageOrPrintOptions
                    chart.ToImage(stream, options);

                    // Visualizza il messaggio di successo
                    Console.WriteLine("Chart successfully converted to image with custom options");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Salva la cartella di lavoro
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

### Vedi anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


