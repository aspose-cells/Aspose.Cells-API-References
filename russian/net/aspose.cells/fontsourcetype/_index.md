---
title: "Перечисление FontSourceType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.FontSourceType. Указывает тип источника шрифта"
type: docs
url: /ru/net/aspose.cells/fontsourcetype/
---
## FontSourceType enumeration

Указывает тип источника шрифта.

```csharp
public enum FontSourceType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| FontFile | `0` | представляет один файл шрифта. |
| FontsFolder | `1` | Представляет папку с файлами шрифтов. |
| MemoryFont | `2` | Представляет один шрифт в памяти. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontSourceTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Продемонстрировать значения перечисления FontSourceType
            Console.WriteLine("FontSourceType values:");
            Console.WriteLine($"FontFile: {FontSourceType.FontFile}");
            Console.WriteLine($"FontsFolder: {FontSourceType.FontsFolder}");
            Console.WriteLine($"MemoryFont: {FontSourceType.MemoryFont}");

            // Создать настройки шрифта и использовать FontSourceType
            FontConfigs.SetFontFolder(@"C:\MyFonts\", false);
            FontConfigs.SetFontSources(new FontSourceBase[]
            {
                new FolderFontSource(@"C:\MyFonts\", false),
                new FileFontSource(@"C:\MyFonts\arial.ttf"),
                new MemoryFontSource(new byte[0])
            });

            // Применить шрифт к ячейке
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with Arial font");

            // Сохранить результат
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


