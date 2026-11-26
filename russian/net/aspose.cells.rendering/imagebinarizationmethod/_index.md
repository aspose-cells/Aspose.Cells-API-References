---
title: "Перечисление ImageBinarizationMethod"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Rendering.ImageBinarizationMethod. Указывает метод, используемый для бинаризации изображения"
type: docs
url: /ru/net/aspose.cells.rendering/imagebinarizationmethod/
---
## ImageBinarizationMethod enumeration

Указывает метод, используемый для бинаризации изображения.

```csharp
public enum ImageBinarizationMethod
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Threshold | `0` | Указывает метод пороговой обработки. |
| FloydSteinbergDithering | `1` | Указывает дизеринг с использованием метода диффузии ошибки Флойда‑Штайнберга. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class RenderingClassImageBinarizationMethodDemo
    {
        public static void Run()
        {
            // Создайте новую рабочую книгу с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните ячейки градиентными значениями для демонстрации
            for (int row = 0; row < 50; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue((double)(row * col) / 500);
                }
            }

            // Настройте параметры рендеринга изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4,
                TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering
            };

            // Создайте рендер листа с настроенными параметрами
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // Отрендерьте первую страницу листа в изображение с бинаризацией
            renderer.ToImage(0, "BinarizedOutput.tiff");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


