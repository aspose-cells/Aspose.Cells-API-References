---
title: "FontFileDataInfo.FormatType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontFileDataInfo. Получает тип формата шрифта файла"
type: docs
url: /ru/net/aspose.cells/fontfiledatainfo/formattype/
---
## FontFileDataInfo.FormatType property

Получает тип формата файла шрифта.

```csharp
public FontFileFormatType FormatType { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyFormatTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте немного текста, чтобы продемонстрировать использование шрифта
            worksheet.Cells["A1"].PutValue("Sample Text with Font");

            try
            {
                // Загрузите пример файла шрифта (замените реальным путем к файлу шрифта)
                string fontFilePath = "arial.ttf";
                if (File.Exists(fontFilePath))
                {
                    // Зарегистрируйте папку со шрифтами
                    FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);

                    // В реальном сценарии FontFileDataInfo будет получен из библиотеки
                    // Для демонстрации мы смоделируем получение информации о шрифте
                    // Примечание: Реальный API может предоставлять это через FontConfigs или аналогичный механизм
                    FontFileDataInfo fontInfo = GetFontFileDataInfo(fontFilePath);

                    if (fontInfo != null)
                    {
                        // Отобразите значение свойства FormatType
                        Console.WriteLine("Font Format Type: " + fontInfo.FormatType);

                        // Покажите значение перечисления в виде строки
                        Console.WriteLine("Format Type Description: " +
                            Enum.GetName(typeof(FontFileFormatType), fontInfo.FormatType));

                        // Примените шрифт к ячейке (концептуально — реальная реализация может отличаться)
                        Style style = worksheet.Cells["A1"].GetStyle();
                        style.Font.Name = "Arial";
                        worksheet.Cells["A1"].SetStyle(style);
                    }
                    else
                    {
                        Console.WriteLine("Font information could not be retrieved");
                    }
                }
                else
                {
                    Console.WriteLine("Font file not found at: " + fontFilePath);
                }

                // Сохраните книгу
                workbook.Save("FormatTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Вспомогательный метод для имитации получения FontFileDataInfo
        // В реальном использовании это будет предоставлено API Aspose.Cells
        private static FontFileDataInfo GetFontFileDataInfo(string fontPath)
        {
            try
            {
                byte[] fontData = File.ReadAllBytes(fontPath);
                string extension = Path.GetExtension(fontPath).ToLower();

                // Создайте макет FontFileDataInfo (на самом деле он будет получен из API)
                // Поскольку мы не можем создать его напрямую, мы смоделируем поведение
                FontFileFormatType formatType = FontFileFormatType.Unknown;

                if (extension == ".ttf")
                    formatType = FontFileFormatType.Ttf;
                else if (extension == ".otf")
                    formatType = FontFileFormatType.Otf;
                else if (extension == ".ttc")
                    formatType = FontFileFormatType.Ttc;

                // В реальной реализации это будет возвращено API
                // Для этой демонстрации мы просто вернём null, так как не можем создать объект
                Console.WriteLine($"Detected font format: {formatType}");
                return null;
            }
            catch
            {
                return null;
            }
        }
    }
}
```

### См. также

* enum [FontFileFormatType](../../fontfileformattype/)
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


