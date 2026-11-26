---
title: "DataBar.ToImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DataBar. Отрисовать полосу данных в ячейке в массив байтов изображения"
type: docs
url: /ru/net/aspose.cells/databar/toimage/
---
## DataBar.ToImage method

Отрисовать data bar в ячейке в массив байтов изображения.

```csharp
public byte[] ToImage(Cell cell, ImageOrPrintOptions imgOpts)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ячейка | Ячейка | Укажите, в какой ячейке должна быть отрисована полоса данных |
| imgOpts | ImageOrPrintOptions | ImageOrPrintOptions содержит некоторые свойства выходного изображения |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class DataBarMethodToImageWithCellImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные и условное форматирование
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            
            // Добавить условное форматирование полос данных
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            idx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcc[idx];
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            
            // Получите ячейку с условным форматированием
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            if (result != null && result.ConditionalFormattingDataBar != null)
            {
                DataBar bar = result.ConditionalFormattingDataBar;
                ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
                
                // Преобразовать полосу данных в изображение
                byte[] img = bar.ToImage(cell, imgOpts);
                
                // Сохраните изображение
                string outputPath = "DataBarImage.png";
                File.WriteAllBytes(outputPath, img);
                
                // Для проверки изображения вам потребуется добавить пакет System.Drawing.Common
                // и использовать System.Drawing.Image при необходимости
                Console.WriteLine($"Data bar image saved to {outputPath}");
            }
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


