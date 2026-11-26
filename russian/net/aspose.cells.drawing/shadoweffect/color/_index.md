---
title: "ShadowEffect.Color"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShadowEffect. Получает и задает цвет тени"
type: docs
url: /ru/net/aspose.cells.drawing/shadoweffect/color/
---
## ShadowEffect.Color property

Получает и задает цвет тени.

```csharp
public CellsColor Color { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShadowEffectPropertyColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму, чтобы продемонстрировать эффект тени
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Получите эффект тени из формы
                ShadowEffect shadowEffect = shape.ShadowEffect;

                // Создайте новый объект CellsColor
                CellsColor shadowColor = workbook.CreateCellsColor();

                // Установите цвет красным, используя значения RGB
                shadowColor.Color = Color.Red;

                // Примените цвет к эффекту тени
                shadowEffect.Color = shadowColor;

                // Отобразите текущее значение цвета
                Console.WriteLine("Shadow Color (RGB): " + shadowEffect.Color.Color.ToString());
                Console.WriteLine("Shadow Color (ARGB): " + shadowEffect.Color.Argb);

                // Сохраните рабочую книгу, чтобы продемонстрировать эффект
                workbook.Save("ShadowEffectColorDemo.xlsx");

                // Загрузите книгу обратно, чтобы проверить, что цвет был сохранён
                Workbook loadedWorkbook = new Workbook("ShadowEffectColorDemo.xlsx");
                ShadowEffect loadedShadowEffect = loadedWorkbook.Worksheets[0].Shapes[0].ShadowEffect;

                // Отобразите загруженное значение цвета
                Console.WriteLine("Loaded Shadow Color (RGB): " + loadedShadowEffect.Color.Color.ToString());
                Console.WriteLine("Loaded Shadow Color (ARGB): " + loadedShadowEffect.Color.Argb);
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


