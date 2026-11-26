---
title: "ImageOrPrintOptions.SetDesiredSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ImageOrPrintOptions. Establece el ancho y la altura deseados de la imagen"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/setdesiredsize/
---
## SetDesiredSize(int, int) {#setdesiredsize}

Establece el ancho y alto deseados de la imagen.

```csharp
[Obsolete("Use SetDesiredSize(int, int, bool) by setting param keepAspectRatio to false instead.")]
public void SetDesiredSize(int desiredWidth, int desiredHeight)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desiredWidth | Int32 | ancho deseado en píxeles |
| desiredHeight | Int32 | altura deseada en píxeles |

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use `SetDesiredSize` estableciendo el parámetro keepAspectRatio a false. Esta propiedad será eliminada 12 meses después desde mayo de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue(i);
            }

            // Establecer área de impresión
            worksheet.PageSetup.PrintArea = "A1:A11";

            // Crear opciones de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.SetDesiredSize(800, 600); // Using SetDesiredSize with Int32 parameters
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            // Renderiza la hoja de cálculo a una imagen
            SheetRender render = new SheetRender(worksheet, options);
            render.ToImage(0, "output.jpg");

            Console.WriteLine("Image generated with desired size 800x600");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SetDesiredSize(int, int, bool) {#setdesiredsize_1}

Establece el ancho y alto deseados de la imagen.

```csharp
public void SetDesiredSize(int desiredWidth, int desiredHeight, bool keepAspectRatio)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desiredWidth | Int32 | ancho deseado en píxeles |
| desiredHeight | Int32 | altura deseada en píxeles |
| keepAspectRatio | Booleano | si se debe mantener la relación de aspecto de la imagen original |

### Observaciones

El ancho y la altura de la imagen de salida en píxeles se basarán únicamente en el ancho y la altura deseados establecidos.

Los [`HorizontalResolution`](../horizontalresolution/) y [`VerticalResolution`](../verticalresolution/) no afectarán el ancho y la altura de la imagen de salida en este caso.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
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

            // Obtener la forma del gráfico
            Shape chartShape = worksheet.Shapes[0];

            // Establezca opciones de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.SetDesiredSize(800, 600, false); // Using SetDesiredSize with width, height, and keepAspectRatio

            // Guardar el gráfico como imagen
            MemoryStream stream = new MemoryStream();
            chartShape.ToImage(stream, options);

            // Guarda la imagen en un archivo
            File.WriteAllBytes("output_chart.png", stream.ToArray());
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


