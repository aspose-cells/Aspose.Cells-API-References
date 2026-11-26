---
title: "Класс FontConfigs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FontConfigs. Указывает настройки шрифтов"
type: docs
url: /ru/net/aspose.cells/fontconfigs/
---
## FontConfigs class

Указывает настройки шрифта

```csharp
public class FontConfigs
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [FontConfigs](fontconfigs/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| static [DefaultFontName](../../aspose.cells/fontconfigs/defaultfontname/) { get; set; } | Получает или задает имя шрифта по умолчанию. |
| static [PreferSystemFontSubstitutes](../../aspose.cells/fontconfigs/prefersystemfontsubstitutes/) { get; set; } | Указывает, использовать ли сначала системные заменители шрифтов, когда шрифт не представлен и заменитель этого шрифта не установлен. Например, в Ubuntu шрифт \"Arial\" обычно заменяется на \"Liberation Sans\". Значение по умолчанию — false. |

## Методы

| Имя | Описание |
| --- | --- |
| static [GetFontFileDataInfo](../../aspose.cells/fontconfigs/getfontfiledatainfo/)(string, bool, bool, bool) | Получить информацию о данных файла шрифта. |
| static [GetFontSources](../../aspose.cells/fontconfigs/getfontsources/)() | Получает копию массива, содержащего список источников |
| static [GetFontSubstitutes](../../aspose.cells/fontconfigs/getfontsubstitutes/)(string) | Возвращает массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт отсутствует. |
| static [IsFontAvailable](../../aspose.cells/fontconfigs/isfontavailable/)(string) | Указывает, доступен ли шрифт. |
| static [SetFontFolder](../../aspose.cells/fontconfigs/setfontfolder/)(string, bool) | Устанавливает папку шрифтов |
| static [SetFontFolders](../../aspose.cells/fontconfigs/setfontfolders/)(string[], bool) | Устанавливает папку шрифтов |
| static [SetFontSources](../../aspose.cells/fontconfigs/setfontsources/)(FontSourceBase[]) | Устанавливает источники шрифтов. |
| static [SetFontSubstitutes](../../aspose.cells/fontconfigs/setfontsubstitutes/)(string, string[]) | Имена заменяющих шрифтов для заданного оригинального имени шрифта. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontConfigsDemo
    {
        public static void Run()
        {
            // Установить пользовательскую папку шрифтов
            string fontFolder = @"C:\MyFonts\";
            FontConfigs.SetFontFolder(fontFolder, true);

            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить пример текста с разными шрифтами
            worksheet.Cells["A1"].PutValue("Text with default font");
            worksheet.Cells["A2"].PutValue("Text with custom font");
            
            // Применить пользовательский стиль шрифта
            Style style = workbook.CreateStyle();
            style.Font.Name = "MyCustomFont"; // This font should exist in the custom font folder
            worksheet.Cells["A2"].SetStyle(style);

            // Сохранить в HTML для демонстрации отображения шрифтов
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportImagesAsBase64 = true,
                PresentationPreference = true
            };
            
            workbook.Save("output.html", options);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


