---
title: "FontSetting.SetWordArtStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontSetting. Устанавливает предустановленный стиль WordArt"
type: docs
url: /ru/net/aspose.cells/fontsetting/setwordartstyle/
---
## FontSetting.SetWordArtStyle method

Устанавливает предустановленный стиль WordArt.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | PresetWordArtStyle | Предустановленный стиль WordArt. |

### Примечания

Только для текста фигуры/диаграммы.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FontSettingMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторый текст в ячейку A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text for WordArt");

            // Создать настройку шрифта для текста в ячейке A1
            FontSetting fontSetting = new FontSetting(0, cell.StringValue.Length, workbook.Worksheets);

            try
            {
                // Применить стиль WordArt к настройке шрифта
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle3);

                Console.WriteLine("WordArt style applied successfully to the text.");
                
                // Показать эффект, сохранив книгу
                worksheet.AutoFitColumn(0);
                worksheet.AutoFitRow(0);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("FontSettingMethodSetWordArtStyleDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


