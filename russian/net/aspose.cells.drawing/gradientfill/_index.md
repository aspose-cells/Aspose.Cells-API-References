---
title: "Класс GradientFill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.GradientFill. Представляет градиентную заливку"
type: docs
url: /ru/net/aspose.cells.drawing/gradientfill/
---
## GradientFill class

Представляет градиентную заливку.

```csharp
public class GradientFill : Fill
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Angle](../../aspose.cells.drawing/gradientfill/angle/) { get; set; } | Угол линейной заливки. |
| [DirectionType](../../aspose.cells.drawing/gradientfill/directiontype/) { get; } | Получает тип направления градиента. |
| [FillType](../../aspose.cells.drawing/gradientfill/filltype/) { get; } | Получает тип градиентной заливки. |
| [GradientStops](../../aspose.cells.drawing/gradientfill/gradientstops/) { get; } | Представляет коллекцию градиентных остановок. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Унаследовано от [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Получает хеш-код.(Унаследовано от [`Fill`](../fill/).) |
| [SetGradient](../../aspose.cells.drawing/gradientfill/setgradient/)(GradientFillType, double, GradientDirectionType) | Установите тип градиентной заливки и направление. |
| [SetOneColorGradient](../../aspose.cells.drawing/gradientfill/setonecolorgradient/)(Color, double, GradientStyleType, int) | Устанавливает указанное заполнение в одноцветный градиент. Применяется только для Excel 2007. |
| [SetPresetThemeGradient](../../aspose.cells.drawing/gradientfill/setpresetthemegradient/)(PresetThemeGradientType, ThemeColorType) | Устанавливает предустановленную тематическую градиентную заливку. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Устанавливает указанное заполнение в двухцветный градиент. Применяется только для Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Устанавливает указанное заполнение в двухцветный градиент. Применяется только для Excel 2007. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassGradientFillDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную фигуру на лист с всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 150, 100);

            // Установите тип заливки в градиент, чтобы получить доступ к свойствам градиентной заливки
            shape.Fill.FillType = FillType.Gradient;

            // Получите существующий экземпляр градиентной заливки из фигуры
            GradientFill gradientFill = shape.Fill.GradientFill;

            // Настройте градиент с двумя цветами, используя существующий экземпляр
            gradientFill.SetTwoColorGradient(
                Color.LightSkyBlue,  // First color
                Color.DarkBlue,      // Second color
                GradientStyleType.Horizontal, // Gradient style
                1                    // Variant
            );

            // Сохраните книгу
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### См. также

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


