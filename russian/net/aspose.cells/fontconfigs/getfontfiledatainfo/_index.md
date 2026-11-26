---
title: "FontConfigs.GetFontFileDataInfo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontConfigs. Получить информацию о данных файла шрифта"
type: docs
url: /ru/net/aspose.cells/fontconfigs/getfontfiledatainfo/
---
## FontConfigs.GetFontFileDataInfo method

Получить информацию о данных файла шрифта.

```csharp
public static FontFileDataInfo GetFontFileDataInfo(string fontName, bool isBold, bool isItalic, 
    bool isExactStyle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fontName | String | название шрифта |
| isBold | Boolean | стиль шрифта жирный или нет |
| isItalic | Boolean | стиль шрифта курсивный или нет |
| isExactStyle | Boolean | нужно ли точно соответствовать заданному жирному/курсивному стилю |

### Возвращаемое значение

Информация о данных файла шрифта.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontFileDataInfoWithStringBooleanBooleanBooleanDemo
    {
        public static void Run()
        {
            try
            {
                // Вызовите GetFontFileDataInfo с конкретными параметрами (изменено на статический вызов)
                FontFileDataInfo fontInfo = FontConfigs.GetFontFileDataInfo("Arial", true, false, false);

                // Отобразить информацию о данных файлов шрифтов
                if (fontInfo != null)
                {
                    Console.WriteLine($"Font format type: {fontInfo.FormatType}");
                    Console.WriteLine($"Font data length: {fontInfo.Data?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Font information not available");
                }

                // Продемонстрировать эффект на рабочей книге
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Установить стиль с проверенным шрифтом
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.IsBold = true;
                style.Font.IsItalic = false;
                
                // Применить стиль к ячейке
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with Arial Bold");

                // Сохраните книгу
                workbook.Save("FontConfigsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontFileDataInfo method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [FontFileDataInfo](../../fontfiledatainfo/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


