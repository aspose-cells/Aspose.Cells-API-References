---
title: "AutoFitterOptions.AutoFitMergedCellsType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFitterOptions. Получает и задает тип автоподгонки высоты строки объединённых ячеек"
type: docs
url: /ru/net/aspose.cells/autofitteroptions/autofitmergedcellstype/
---
## AutoFitterOptions.AutoFitMergedCellsType property

Получает и задает тип автоматической подгонки высоты строки объединённых ячеек.

```csharp
public AutoFitMergedCellsType AutoFitMergedCellsType { get; set; }
```

### Примечания

Excel по умолчанию игнорирует объединённые ячейки при подборе высоты строки, поэтому Aspose.Cells работает как стандартный режим MS Excel. Пожалуйста, установите этот тип, чтобы изменить способ автоподгонки высоты строки объединённых ячеек.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить примерные данные и объединить ячейки
            worksheet.Cells["A1"].PutValue("This is a sample text for merged cells auto-fit demonstration");
            worksheet.Cells.Merge(0, 0, 3, 2); // Merge A1:B3

            // Автоподгонка строк с AutoFitMergedCellsType.EachLine
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Автоподгонка столбцов с AutoFitMergedCellsType.EachLine
            worksheet.AutoFitColumns(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Сохраните книгу
            workbook.Save("AutoFitMergedCellsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [AutoFitMergedCellsType](../../autofitmergedcellstype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


