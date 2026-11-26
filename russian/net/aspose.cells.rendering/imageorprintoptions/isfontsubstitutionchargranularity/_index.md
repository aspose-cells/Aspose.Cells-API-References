---
title: "ImageOrPrintOptions.IsFontSubstitutionCharGranularity"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Указывает, следует ли заменять шрифт только отдельного символа, когда шрифт ячейки несовместим с ним"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/
---
## ImageOrPrintOptions.IsFontSubstitutionCharGranularity property

Указывает, следует ли заменять шрифт символа только тогда, когда шрифт ячейки несовместим с ним.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Примечания

По умолчанию false. Сначала мы попробуем использовать шрифт по умолчанию из Workbook и PdfSaveOption/system для шрифта ячейки.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsFontSubstitutionCharGranularityDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Настройте ячейку с потенциально неподдерживаемым шрифтом
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with unavailable font");
            Style style = cell.GetStyle();
            style.Font.Name = "NonExistentFont";
            cell.SetStyle(style);

            // Создать параметры рендеринга изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png, // Namespace reference now valid
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = false
            };

            // Отобразите и измените значение свойства
            Console.WriteLine($"Initial IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            
            // Отрендерьте с настройкой по умолчанию
            new SheetRender(worksheet, options).ToImage(0, "BeforeFontSubstitutionChange.png");

            // Измените свойство и отрендерьте снова
            options.IsFontSubstitutionCharGranularity = true;
            Console.WriteLine($"Updated IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            new SheetRender(worksheet, options).ToImage(0, "AfterFontSubstitutionChange.png");

            // Сохраните рабочую книгу для справки
            workbook.Save("FontSubstitutionDemoWorkbook.xlsx");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


