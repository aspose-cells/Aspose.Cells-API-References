---
title: "Chart.ToImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Chart. Obtiene un objeto Bitmap de 32 bits del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Obtiene un objeto `Bitmap` de 32 bits del gráfico.

```csharp
public Bitmap ToImage()
```

### Valor de retorno

la imagen del gráfico.

### Observaciones

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, devolverá null.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["B4"].PutValue(1500);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);
            
            // Convertir el gráfico a imagen y guardar en archivo
            chart.ToImage("ChartImage.png", ImageType.Png);
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Obtiene un objeto `Bitmap` de 32 bits del gráfico. Los atributos `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression y ImageOrPrintOptions.Quality se ignoran.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | ImageOrPrintOptions | Opciones adicionales de creación de imagen |

### Valor de retorno

la imagen del gráfico.

### Observaciones

Devuelve un objeto bitmap de 32 bits, por lo que los atributos ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression y ImageOrPrintOptions.Quality no afectan al método. Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, devolverá null.

### Ejemplos

Obtiene un objeto bitmap con 200 dpi en x y 300 dpi en y.

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

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Crea la imagen del gráfico y la guarda en un archivo. La extensión del nombre del archivo determina el formato de la imagen.

```csharp
public void ToImage(string imageFile)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageFile | String | El nombre del archivo de imagen con ruta completa. |

### Observaciones

El formato de la imagen se especifica mediante la extensión del nombre del archivo. Por ejemplo, si especificas \"myfile.png\", la imagen se guardará en formato PNG. Se reconocen las siguientes extensiones de archivo: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(45);
            worksheet.Cells["B3"].PutValue(55);
            
            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Guardar gráfico como imagen
            chart.ToImage("ChartImage.jpg");
            
            Console.WriteLine("Chart saved as image successfully.");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageFormat) {#toimage_10}

Crea la imagen del gráfico y la guarda en un archivo en el formato especificado.

```csharp
[Obsolete("Use Chart.ToImage(string, ImageType) method instead.")]
public void ToImage(string imageFile, ImageFormat imageFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageFile | String | El nombre del archivo de imagen con ruta completa. |
| imageFormat | ImageFormat | El formato en el que guardar la imagen. |

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utiliza el método Chart.ToImage(string, ImageType). Esta propiedad será eliminada 12 meses después desde julio de 2022. Aspose se disculpa por cualquier inconveniente que puedas haber experimentado.

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Crea la imagen del gráfico y la guarda en un archivo en el tipo de imagen especificado.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageFile | String | El nombre del archivo de imagen con ruta completa. |
| imageType | ImageType | El tipo de imagen en el que guardar la imagen. |

### Observaciones

El tipo de la imagen se especifica usando `imageType`. Los siguientes tipos son compatibles: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(7);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Guardar gráfico como imagen con el ImageType especificado
            chart.ToImage("output_chart.png", ImageType.Png);

            Console.WriteLine("Chart saved to image successfully.");
        }
    }
}
```

### Ver también

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Crea la imagen del gráfico y la guarda en un archivo en formato Jpeg.

```csharp
[Obsolete("Use Chart.ToImage(string,ImageOrPrintOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ToImage(string imageFile, long jpegQuality)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageFile | String | El nombre del archivo de imagen con ruta completa. |
| jpegQuality | Int64 | Calidad Jpeg. |

### Observaciones

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada. NOTA: Este método está ahora obsoleto. En su lugar, utilice el método ToImage(string,ImageOrPrintOptions) con la calidad especificada. Este método será eliminado 12 meses después, a partir de marzo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);
            
            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            try
            {
                // Llame al método ToImage con los parámetros (String, Int64)
                string imagePath = "ChartImage.jpg";
                long jpegQuality = 90; // Quality percentage (0-100)
                chart.ToImage(imagePath, jpegQuality);
                
                Console.WriteLine($"Chart saved as image successfully to: {imagePath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToImage method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ChartToImageDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Crea la imagen del gráfico y la guarda en un flujo en formato Jpeg.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de salida. |
| jpegQuality | Int64 | Calidad Jpeg. |

### Observaciones

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Crear un flujo de memoria para guardar la imagen
                using (MemoryStream stream = new MemoryStream())
                {
                    // Llame al método ToImage con los parámetros Stream e Int64
                    // La calidad JPEG se especifica como 80 (el rango válido suele ser 0-100)
                    chart.ToImage(stream, 80);

                    // Mostrar mensaje de éxito
                    Console.WriteLine("Chart successfully converted to image with JPEG quality 80");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Guarda el libro de trabajo
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

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageFormat) {#toimage_5}

Crea la imagen del gráfico y la guarda en un flujo en el formato especificado.

```csharp
[Obsolete("Use Chart.ToImage(Stream, ImageType) method instead.")]
public void ToImage(Stream stream, ImageFormat imageFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de salida. |
| imageFormat | ImageFormat | El formato en el que guardar la imagen. |

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Chart.ToImage(Stream, ImageType). Esta propiedad será eliminada 12 meses después, a partir de julio de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Crear un flujo de memoria para guardar la imagen
                using (MemoryStream stream = new MemoryStream())
                {
                    // Llame al método ToImage con los parámetros Stream y ImageFormat
                    // Usando Aspose.Cells.Drawing.ImageType en lugar de System.Drawing.Imaging.ImageFormat
                    chart.ToImage(stream, Aspose.Cells.Drawing.ImageType.Png);

                    // Mostrar mensaje de éxito
                    Console.WriteLine("Chart successfully saved to stream in PNG format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // Opcionalmente guarde el flujo en un archivo para verificación
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

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Crea la imagen del gráfico y la guarda en un flujo en el formato especificado.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de salida. |
| imageType | ImageType | El tipo de imagen en el que guardar la imagen. |

### Observaciones

El tipo de la imagen se especifica usando `imageType`. Los siguientes tipos son compatibles: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Crear un flujo de memoria para guardar la imagen
                using (MemoryStream stream = new MemoryStream())
                {
                    // Llame al método ToImage con los parámetros Stream y ImageType
                    chart.ToImage(stream, ImageType.Png);

                    // Mostrar mensaje de éxito
                    Console.WriteLine("Chart successfully converted to image in PNG format");

                    // Guarde la imagen en un archivo para demostración
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
                }

                // Guarda el libro de trabajo
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

### Ver también

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Crea la imagen del gráfico y la guarda en un archivo. La extensión del nombre del archivo determina el formato de la imagen.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageFile | String | El nombre del archivo de imagen con ruta completa. |
| opciones | ImageOrPrintOptions | Opciones adicionales de creación de imagen |

### Observaciones

El formato de la imagen se especifica mediante la extensión del nombre del archivo. Por ejemplo, si especificas \"myfile.png\", la imagen se guardará en formato PNG. Se reconocen las siguientes extensiones de archivo: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada. Por favor, consulte la [Lista de Gráficos Compatibles](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) para más detalles.

### Ejemplos

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
            // Crear opciones de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            options.TiffCompression = TiffCompression.CompressionCCITT4;

            // Cargar el libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra y crear un gráfico
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

            // Guardar gráfico como imagen
            chart.ToImage("chart.tiff", options);
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Crea la imagen del gráfico y la guarda en un flujo en el formato especificado.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de salida. |
| opciones | ImageOrPrintOptions | Opciones adicionales de creación de imagen |

### Observaciones

El tipo de imagen se especifica usando `options.ImageType`. Los siguientes formatos son compatibles: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Si el ancho o la altura es cero o el gráfico no es compatible según la Lista de Gráficos Compatibles, este método no hará nada. Por favor, consulte la [Lista de Gráficos Compatibles](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) para más detalles.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Crear un flujo de memoria para guardar la imagen
                using (MemoryStream stream = new MemoryStream())
                {
                    // Cree ImageOrPrintOptions con configuraciones específicas
                    ImageOrPrintOptions options = new ImageOrPrintOptions();
                    options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                    options.HorizontalResolution = 300;
                    options.VerticalResolution = 300;

                    // Llame al método ToImage con los parámetros Stream y ImageOrPrintOptions
                    chart.ToImage(stream, options);

                    // Mostrar mensaje de éxito
                    Console.WriteLine("Chart successfully converted to image with custom options");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Guarda el libro de trabajo
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

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


