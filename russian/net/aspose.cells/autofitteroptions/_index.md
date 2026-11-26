---
title: "Класс AutoFitterOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.AutoFitterOptions. Представляет все параметры автоподгонки."
type: docs
url: /ru/net/aspose.cells/autofitteroptions/
---
## AutoFitterOptions class

Представляет все параметры автофиттера.

```csharp
public class AutoFitterOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [AutoFitterOptions](autofitteroptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoFitMergedCells](../../aspose.cells/autofitteroptions/autofitmergedcells/) { get; set; } | (**Obsolete.**) Указывает, следует ли автоматически подгонять высоту строки, когда ячейки объединены в строке. Значение по умолчанию — false. |
| [AutoFitMergedCellsType](../../aspose.cells/autofitteroptions/autofitmergedcellstype/) { get; set; } | Получает и задает тип автоматической подгонки высоты строки объединённых ячеек. |
| [AutoFitWrappedTextType](../../aspose.cells/autofitteroptions/autofitwrappedtexttype/) { get; set; } | Получает и задает тип автоматической подгонки перенесённого текста. |
| [DefaultEditLanguage](../../aspose.cells/autofitteroptions/defaulteditlanguage/) { get; set; } | Получает или задает язык редактирования по умолчанию. |
| [FormatStrategy](../../aspose.cells/autofitteroptions/formatstrategy/) { get; set; } | Получает и задает стратегию форматирования. |
| [ForRendering](../../aspose.cells/autofitteroptions/forrendering/) { get; set; } | Указывает, следует ли подгонка для целей рендеринга. |
| [IgnoreHidden](../../aspose.cells/autofitteroptions/ignorehidden/) { get; set; } | Игнорирует скрытые строки/столбцы. |
| [MaxRowHeight](../../aspose.cells/autofitteroptions/maxrowheight/) { get; set; } | Получает и задает максимальную высоту строки (в единицах Point) при автоматической подгонке строк. |
| [OnlyAuto](../../aspose.cells/autofitteroptions/onlyauto/) { get; set; } | Указывает, следует ли подгонять только те строки, высота которых не задана вручную. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitterOptionsDemo
    {
        public static void AutoFitterOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and autofitted.");

            Style style = worksheet.Cells["A1"].GetStyle();

            style.IsTextWrapped = true;

            worksheet.Cells["A1"].SetStyle(style);

            // Создать диапазон A1:B2
            Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);

            // Объедините ячейки
            range.Merge();

            // Создайте экземпляр AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                DefaultEditLanguage = DefaultEditLanguage.English,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                OnlyAuto = true,
                IgnoreHidden = true,
                MaxRowHeight = 50.0,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                ForRendering = true
            };

            // Примените автоматическую подгонку строк с указанными параметрами
            worksheet.AutoFitRows(options);

            // Сохраните книгу
            workbook.Save("AutoFitterOptionsExample.xlsx");
            workbook.Save("AutoFitterOptionsExample.pdf");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


