---
title: "Перечисление ChartColorPaletteType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.ChartColorPaletteType. Перечисляет все монохромные палитры, используемые в диаграмме Excel"
type: docs
url: /ru/net/aspose.cells.charts/chartcolorpalettetype/
---
## ChartColorPaletteType enumeration

Перечисляет все монохромные палитры, используемые в диаграмме Excel.

```csharp
public enum ChartColorPaletteType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| MonochromaticPalette1 | `1` | Градиент цвета темы accent1, от тёмного к светлому. |
| MonochromaticPalette2 | `2` | Градиент цвета темы accent2, от тёмного к светлому. |
| MonochromaticPalette3 | `3` | Градиент цвета темы accent3, от тёмного к светлому. |
| MonochromaticPalette4 | `4` | Градиент цвета темы accent4, от тёмного к светлому. |
| MonochromaticPalette5 | `5` | Градиент цвета темы accent5, от тёмного к светлому. |
| MonochromaticPalette6 | `6` | Градиент цвета темы accent6, от тёмного к светлому. |
| MonochromaticPalette7 | `7` | Градиент цвета темы accent7. |
| MonochromaticPalette8 | `8` | Градиент цвета темы accent1, от светлого к тёмному. |
| MonochromaticPalette9 | `9` | Градиент цвета темы accent2, от светлого к тёмному. |
| MonochromaticPalette10 | `10` | Градиент цвета темы accent3, от светлого к тёмному. |
| MonochromaticPalette11 | `11` | Градиент цвета темы accent4, от светлого к тёмному. |
| MonochromaticPalette12 | `12` | Градиент цвета темы accent5, от светлого к тёмному. |
| MonochromaticPalette13 | `13` | Градиент цвета темы accent6, от светлого к тёмному. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartColorPaletteTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте пример диаграммы, чтобы продемонстрировать цветовую палитру
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Продемонстрируйте использование разных значений перечисления ChartColorPaletteType
                ChartColorPaletteType palette1 = ChartColorPaletteType.MonochromaticPalette1;
                ChartColorPaletteType palette5 = ChartColorPaletteType.MonochromaticPalette5;
                ChartColorPaletteType palette8 = ChartColorPaletteType.MonochromaticPalette8;

                // Отобразить значения перечисления
                Console.WriteLine($"MonochromaticPalette1 value: {(int)palette1}");
                Console.WriteLine($"MonochromaticPalette5 value: {(int)palette5}");
                Console.WriteLine($"MonochromaticPalette8 value: {(int)palette8}");

                // Сохраните книгу
                workbook.Save("ChartColorPaletteTypeDemo.xlsx");
                Console.WriteLine("ChartColorPaletteType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ChartColorPaletteType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


