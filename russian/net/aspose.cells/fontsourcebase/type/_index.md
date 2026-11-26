---
title: "FontSourceBase.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontSourceBase. Возвращает тип источника шрифта"
type: docs
url: /ru/net/aspose.cells/fontsourcebase/type/
---
## FontSourceBase.Type property

Возвращает тип источника шрифтов.

```csharp
public abstract FontSourceType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSourceBasePropertyTypeDemo
    {
        public static void Run()
        {
            // Создать экземпляр рабочей книги
            Workbook workbook = new Workbook();
            
            // Создать источник шрифтов из папки
            FolderFontSource folderFontSource = new FolderFontSource("C:\\MyFonts", true);
            
            // Отобразить свойство Type источника шрифта
            Console.WriteLine("Font source type: " + folderFontSource.Type);
            
            // Создать файловый источник шрифта
            FileFontSource fileFontSource = new FileFontSource("arial.ttf");
            
            // Отобразить свойство Type источника шрифта
            Console.WriteLine("Font source type: " + fileFontSource.Type);
            
            // Создать источник шрифта в памяти (пример с массивом байтов)
            byte[] fontData = System.IO.File.ReadAllBytes("arial.ttf");
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);
            
            // Отобразить свойство Type источника шрифта
            Console.WriteLine("Font source type: " + memoryFontSource.Type);
            
            // Установить источники шрифтов с помощью статического метода
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource, fileFontSource, memoryFontSource });
            
            // Сохраните книгу
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FontSourceType](../../fontsourcetype/)
* class [FontSourceBase](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


