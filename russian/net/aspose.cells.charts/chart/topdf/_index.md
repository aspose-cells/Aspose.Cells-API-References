---
title: "Chart.ToPdf"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Chart. Сохраняет диаграмму в pdf-файл"
type: docs
url: /ru/net/aspose.cells.charts/chart/topdf/
---
## ToPdf(string) {#topdf_2}

Сохраняет диаграмму в pdf‑файл.

```csharp
public void ToPdf(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | имя pdf-файла с полным путем |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Экспортировать диаграмму в PDF
            chart.ToPdf("output_chart.pdf");
            
            Console.WriteLine("Chart exported to PDF successfully.");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_3}

Сохраняет диаграмму в pdf‑файл.

```csharp
public void ToPdf(string fileName, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | имя pdf-файла с полным путем |
| desiredPageWidth | Single | Желаемая ширина страницы в дюймах. |
| desiredPageHeight | Single | Желаемая высота страницы в дюймах. |
| hAlignmentType | PageLayoutAlignmentType | Тип горизонтального выравнивания диаграммы на выходной странице. |
| vAlignmentType | PageLayoutAlignmentType | Тип вертикального выравнивания диаграммы на выходной странице. |

### Примеры

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

### См. также

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(Stream) {#topdf}

Создаёт PDF диаграммы и сохраняет его в поток.

```csharp
public void ToPdf(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Выходной поток. |

### Примеры

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
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить диаграмму некоторыми образцовыми данными
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(45);
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["B4"].PutValue(25);

            // Добавить столбчатую диаграмму на лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить источник данных для диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Экспортировать диаграмму в PDF с использованием FileStream
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

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_1}

Создаёт pdf диаграммы и сохраняет его в поток.

```csharp
public void ToPdf(Stream stream, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Выходной поток. |
| desiredPageWidth | Single | Желаемая ширина страницы в дюймах. |
| desiredPageHeight | Single | Желаемая высота страницы в дюймах. |
| hAlignmentType | PageLayoutAlignmentType | Тип горизонтального выравнивания диаграммы на выходной странице. |
| vAlignmentType | PageLayoutAlignmentType | Тип вертикального выравнивания диаграммы на выходной странице. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Создайте поток памяти для сохранения PDF
                using (MemoryStream stream = new MemoryStream())
                {
                    // Вызовите метод ToPdf с параметрами Stream, Single, Single, PageLayoutAlignmentType, PageLayoutAlignmentType
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

            // Сохраните книгу
            workbook.Save("ChartToPdfDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


