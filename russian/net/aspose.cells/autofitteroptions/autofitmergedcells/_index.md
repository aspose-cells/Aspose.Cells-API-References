---
title: "AutoFitterOptions.AutoFitMergedCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFitterOptions. Указывает, следует ли автоматически подгонять высоту строки, когда ячейки объединены в строке. Значение по умолчанию — false."
type: docs
url: /ru/net/aspose.cells/autofitteroptions/autofitmergedcells/
---
## AutoFitterOptions.AutoFitMergedCells property

Указывает, следует ли автоматически подгонять высоту строки, когда ячейки объединены в строке. Значение по умолчанию — false.

```csharp
[Obsolete("Use AutoFitterOptions.AutoFitMergedCellsType property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AutoFitMergedCells { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство AutoFitterOptions.AutoFitMergedCellsType. Это свойство будет удалено через 12 месяцев, начиная с декабря 2018 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте примерные данные и объедините ячейки
            worksheet.Cells["A1"].PutValue("This is a test of AutoFitMergedCells property");
            worksheet.Cells.Merge(0, 0, 3, 3); // Merge cells A1:C3

            // Создайте AutoFitterOptions и установите AutoFitMergedCells
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;

            // Автоподгонка строк с объединёнными ячейками
            worksheet.AutoFitRows(options);

            // Сохраните книгу
            workbook.Save("AutoFitMergedCellsExample.xlsx");
        }
    }
}
```

### См. также

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


