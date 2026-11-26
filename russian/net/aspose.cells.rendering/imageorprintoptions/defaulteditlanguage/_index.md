---
title: "ImageOrPrintOptions.DefaultEditLanguage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Возвращает или задает язык редактирования по умолчанию"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/
---
## ImageOrPrintOptions.DefaultEditLanguage property

Получает или задает язык редактирования по умолчанию.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Примечания

Он может отображать/рендерить разные макеты абзаца текста при установленном различном языке редактирования. По умолчанию — Auto.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Установите шрифт по умолчанию книги, поддерживающий символы CJK
            workbook.DefaultStyle.Font.Name = "MS Gothic";
            
            // Установите японский текст, требующий правильного переноса
            string japaneseText = "日本語のテキストサンプル：これは折り返し表示のテストです。長いテキストをセル内で適切に表示するか確認します。";
            sheet.Cells["A1"].Value = japaneseText;
            
            // Настройте форматирование ячеек — исправлено с использованием правильного имени свойства
            Cell cell = sheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;  // Correct property name for text wrapping
            cell.SetStyle(style);
            
            sheet.Cells.SetColumnWidth(0, 15);
            sheet.Cells.SetRowHeight(0, 60);

            // Создать параметры рендеринга изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.CheckWorkbookDefaultFont = true;

            // Отрисовать лист в изображение
            SheetRender renderer = new SheetRender(sheet, options);
            renderer.ToImage(0, "CJK_Text_Rendering.png");
            
            Console.WriteLine("Generated image with CJK text rendering.");
        }
    }
}
```

### См. также

* enum [DefaultEditLanguage](../../../aspose.cells/defaulteditlanguage/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


