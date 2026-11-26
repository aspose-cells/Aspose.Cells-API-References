---
title: "ImageOrPrintOptions.ChartImageType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Указывает тип изображения диаграммы при конвертации. значение по умолчанию PNG"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/chartimagetype/
---
## ImageOrPrintOptions.ChartImageType property

Указывает тип изображения диаграммы при конвертации. значение по умолчанию: PNG.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ChartImageType { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого диаграммы и фигуры всегда рендерятся как векторные элементы (например, точка, линия) для обеспечения качества отображения. Это свойство будет удалено через 12 месяцев, начиная с июня 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyChartImageTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить лист с диаграммой
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:A4", true);

            try
            {
                // Создайте экземпляр ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Отобразить текущее значение ChartImageType
                Console.WriteLine("Current ChartImageType: " + options.ImageType);

                // Установить другой тип изображения для рендеринга диаграммы
                options.ImageType = ImageType.Png;
                Console.WriteLine("ChartImageType set to: " + options.ImageType);

                // Создать SheetRender, чтобы продемонстрировать эффект свойства
                SheetRender renderer = new SheetRender(worksheet, options);

                // Отобразить диаграмму в поток памяти
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Chart rendered successfully with ChartImageType: " + options.ImageType);
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Сохраните книгу
                workbook.Save("ChartImageTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


