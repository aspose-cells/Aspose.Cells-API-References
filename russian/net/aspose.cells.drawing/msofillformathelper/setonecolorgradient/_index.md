---
title: "MsoFillFormatHelper.SetOneColorGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод MsoFillFormatHelper. Устанавливает указанную заливку в одноцветный градиент"
type: docs
url: /ru/net/aspose.cells.drawing/msofillformathelper/setonecolorgradient/
---
## MsoFillFormatHelper.SetOneColorGradient method

Устанавливает указанное заполнение в градиент из одного цвета.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| цвет | Color | Один цвет градиента. |
| степень | Double | Степень градиента. Может принимать значение от 0.0 (тёмный) до 1.0 (светлый). |
| стиль | GradientStyleType | Стиль затенения градиента. |
| variant | Int32 | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Разместите простую метку в листе для контекста
            worksheet.Cells["A1"].Value = "Gradient Fill Demo";

            try
            {
                // Создайте экземпляр MsoFillFormatHelper с помощью рефлексии (нет публичного конструктора)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Параметры градиента
                Color gradientColor = Color.FromArgb(255, 0, 120, 215); // a shade of blue
                double degree = 45.0;                                 // gradient angle in degrees
                GradientStyleType style = GradientStyleType.Horizontal; // horizontal gradient
                int variant = 0;                                      // variant (0 = default)

                // Примените одноцветный градиент
                fillHelper.SetOneColorGradient(gradientColor, degree, style, variant);

                // Опционально: покажите, что свойства могут быть прочитаны после вызова
                Console.WriteLine($"ForeColor after gradient: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency after gradient: {fillHelper.ForeColorTransparency}");

                // Сохраните книгу (визуальных изменений не будет видно, потому что помощник не привязан к фигуре)
                workbook.Save("SetOneColorGradientDemo.xlsx");

                Console.WriteLine("SetOneColorGradient method called successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


