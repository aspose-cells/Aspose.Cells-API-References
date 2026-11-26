---
title: "Перечисление GradientPresetType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.GradientPresetType. Представляет тип предустановленного градиентного цвета"
type: docs
url: /ru/net/aspose.cells.drawing/gradientpresettype/
---
## GradientPresetType enumeration

Представляет тип предустановленного цвета градиента.

```csharp
public enum GradientPresetType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Brass | `0` | Предустановленный цвет латунный |
| CalmWater | `1` | Предустановленный цвет спокойной воды |
| Chrome | `2` | Предустановленный цвет хрома |
| ChromeII | `3` | Предустановленный цвет хром II |
| Daybreak | `4` | Предустановленный цвет рассвета |
| Desert | `5` | Предустановленный цвет пустыни |
| EarlySunset | `6` | Предустановленный цвет раннего заката |
| Fire | `7` | Предустановленный цвет огня |
| Fog | `8` | Предустановленный цвет тумана |
| Gold | `9` | Предустановленный цвет золота |
| GoldII | `10` | Предустановленный цвет золото II |
| Horizon | `11` | Предустановленный цвет горизонта |
| LateSunset | `12` | Предустановленный цвет позднего заката |
| Mahogany | `13` | Предустановленный цвет красного дерева |
| Moss | `14` | Предустановочный цвет мха |
| Nightfall | `15` | Предустановочный цвет заката |
| Ocean | `16` | Предустановочный цвет океана |
| Parchment | `17` | Предустановочный цвет пергамента |
| Peacock | `18` | Предустановочный цвет павлина |
| Rainbow | `19` | Предустановочный цвет радуги |
| RainbowII | `20` | Предустановочный цвет радуги II |
| Sapphire | `21` | Предустановочный цвет сапфира |
| Silver | `22` | Предустановочный цвет серебра |
| Wheat | `23` | Предустановочный цвет пшеницы |
| Unknown | `24` | Неизвестный предустановочный цвет. Используется только для предустановочного цвета (который не совпадает ни с одним известным предустановочным цветом) в шаблонной рабочей книге. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientPresetTypeDemo
    {
        public static void GradientPresetTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Получить доступ к категориальной оси диаграммы
            Axis categoryAxis = chart.CategoryAxis;

            // Получить доступ к формату заливки области категориальной оси
            FillFormat fillFormat = categoryAxis.Area.FillFormat;

            // Установить градиентный предустановочный цвет для формата заливки
            fillFormat.SetPresetColorGradient(GradientPresetType.Fire, GradientStyleType.Horizontal, 1);

            // Вывести тип градиентного предустановочного цвета
            Console.WriteLine("Gradient Preset Color: " + fillFormat.PresetColor);

            // Сохраните книгу
            workbook.Save("GradientPresetTypeExample.xlsx");
            workbook.Save("GradientPresetTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


