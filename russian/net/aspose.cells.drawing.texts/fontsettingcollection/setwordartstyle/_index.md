---
title: "FontSettingCollection.SetWordArtStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontSettingCollection. Устанавливает предустановленный стиль WordArt"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/
---
## FontSettingCollection.SetWordArtStyle method

Устанавливает предустановленный стиль WordArt.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | PresetWordArtStyle | Предустановленный стиль WordArt. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Устанавливает начальный текст
            fontSettingCollection.Text = "Sample Text for WordArt Styling";

            try
            {
                // Вызовите метод SetWordArtStyle с параметром WordArtStyle7 (Градиентная заливка — синяя, акцент 1, отражение)
                fontSettingCollection.SetWordArtStyle(PresetWordArtStyle.WordArtStyle7);

                Console.WriteLine("WordArt style applied successfully to the text box.");

                // Сохраните книгу, чтобы показать эффект
                workbook.Save("FontSettingCollectionSetWordArtStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


