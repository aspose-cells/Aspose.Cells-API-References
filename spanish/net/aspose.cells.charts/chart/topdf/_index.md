---
title: "Chart.ToPdf"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Chart. Guarda el gráfico en un archivo pdf"
type: docs
url: /es/net/aspose.cells.charts/chart/topdf/
---
## ToPdf(string) {#topdf_2}

Guarda el gráfico en un archivo PDF.

```csharp
public void ToPdf(string fileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | el nombre del archivo pdf con ruta completa |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToPdfWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo y agregue datos de muestra
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Exportar el gráfico a PDF
            chart.ToPdf("output_chart.pdf");
            
            Console.WriteLine("Chart exported to PDF successfully.");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_3}

Guarda el gráfico en un archivo PDF.

```csharp
public void ToPdf(string fileName, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | el nombre del archivo pdf con ruta completa |
| desiredPageWidth | Single | El ancho de página deseado en pulgadas. |
| desiredPageHeight | Single | La altura de página deseada en pulgadas. |
| hAlignmentType | PageLayoutAlignmentType | El tipo de alineación horizontal del gráfico en la página de salida. |
| vAlignmentType | PageLayoutAlignmentType | El tipo de alineación vertical del gráfico en la página de salida. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToPdfWithStringSingleSinglePageLayoutAlDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:A4", true);
            chart.Title.Text = "Demo Chart";

            chart.ToPdf("ChartDemo.pdf", 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);
        }
    }
}
```

### Ver también

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(Stream) {#topdf}

Crea el PDF del gráfico y lo guarda en un flujo.

```csharp
public void ToPdf(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de salida. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToPdfWithStreamDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(45);
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["B4"].PutValue(25);

            // Agregar un gráfico de columnas a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establece la fuente de datos para el gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Exportar el gráfico a un PDF usando un FileStream
                using (FileStream pdfStream = new FileStream("ChartOutput.pdf", FileMode.Create, FileAccess.Write))
                {
                    chart.ToPdf(pdfStream);
                }

                Console.WriteLine("Chart successfully exported to ChartOutput.pdf");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error exporting chart to PDF: {ex.Message}");
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

## ToPdf(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_1}

Crea el PDF del gráfico y lo guarda en un flujo.

```csharp
public void ToPdf(Stream stream, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de salida. |
| desiredPageWidth | Single | El ancho de página deseado en pulgadas. |
| desiredPageHeight | Single | La altura de página deseada en pulgadas. |
| hAlignmentType | PageLayoutAlignmentType | El tipo de alineación horizontal del gráfico en la página de salida. |
| vAlignmentType | PageLayoutAlignmentType | El tipo de alineación vertical del gráfico en la página de salida. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToPdfWithStreamSingleSinglePageLayoutAl115534Demo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Crear un flujo de memoria para guardar el PDF
                using (MemoryStream stream = new MemoryStream())
                {
                    // Llamar al método ToPdf con los parámetros Stream, Single, Single, PageLayoutAlignmentType, PageLayoutAlignmentType
                    float desiredPageWidth = 8.5f; // 8.5 inches
                    float desiredPageHeight = 11f; // 11 inches
                    PageLayoutAlignmentType hAlignment = PageLayoutAlignmentType.Center;
                    PageLayoutAlignmentType vAlignment = PageLayoutAlignmentType.Center;

                    chart.ToPdf(stream, desiredPageWidth, desiredPageHeight, hAlignment, vAlignment);

                    Console.WriteLine("Chart successfully converted to PDF in memory stream.");
                    Console.WriteLine($"PDF stream length: {stream.Length} bytes");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to PDF: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("ChartToPdfDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


