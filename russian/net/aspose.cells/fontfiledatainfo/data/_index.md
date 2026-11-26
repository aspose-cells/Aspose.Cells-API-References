---
title: "FontFileDataInfo.Data"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontFileDataInfo. Получает двоичные данные файла шрифта"
type: docs
url: /ru/net/aspose.cells/fontfiledatainfo/data/
---
## FontFileDataInfo.Data property

Получает двоичные данные файла шрифта.

```csharp
public byte[] Data { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Загрузите файл шрифта (замените реальным путем к файлу шрифта)
            string fontFilePath = "samplefont.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Создайте экземпляр FontConfigs и добавьте шрифт
            FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);
            
            // В реальном использовании FontFileDataInfo будет получен из библиотеки
            // Для демонстрационных целей мы просто покажем, как вы бы использовали его, если бы он у вас был
            FontFileDataInfo fontInfo = null; // Normally obtained from library APIs
            
            // Отобразите информацию о данных шрифта (если доступно)
            Console.WriteLine("Font data length: " + (fontInfo?.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
            }

            // В реальном использовании свойство Data будет использоваться для доступа к двоичным данным шрифта
            // Например, вы можете сохранить его в файл:
            if (fontInfo?.Data != null && fontInfo.Data.Length > 0)
            {
                File.WriteAllBytes("extracted_font.ttf", fontInfo.Data);
                Console.WriteLine("Font data extracted to file.");
            }

            // Сохраните книгу (шрифт будет влиять на рендеринг, если используется в ячейках)
            workbook.Save("FontDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


