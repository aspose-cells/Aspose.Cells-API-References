---
title: "Title.Characters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Title. Получает форматирование текста этого заголовка"
type: docs
url: /ru/net/aspose.cells.charts/title/characters/
---
## Title.Characters method

Получает форматирование текста этого заголовка.

```csharp
public FontSetting[] Characters()
```

### Возвращаемое значение

возвращает массив FontSetting

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitleMethodCharactersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["B3"].PutValue(5);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Установить заголовок диаграммы
            chart.Title.Text = "Fruit Sales Report";
            chart.Title.IsVisible = true;

            try
            {
                // Получить форматирование текста заголовка
                FontSetting[] titleCharacters = chart.Title.Characters();
                
                // Изменить шрифт первого символа
                if (titleCharacters.Length > 0)
                {
                    titleCharacters[0].Font.Color = System.Drawing.Color.Red;
                    titleCharacters[0].Font.IsBold = true;
                    titleCharacters[0].Font.Size = 14;
                }

                Console.WriteLine("Characters method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Characters method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("TitleMethodCharactersDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


