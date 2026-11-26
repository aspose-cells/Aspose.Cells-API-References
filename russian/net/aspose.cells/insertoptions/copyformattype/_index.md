---
title: "InsertOptions.CopyFormatType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство InsertOptions."
type: docs
url: /ru/net/aspose.cells/insertoptions/copyformattype/
---
## InsertOptions.CopyFormatType property

```csharp
public CopyFormatType CopyFormatType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyCopyFormatTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Задайте значения и форматирование для демонстрации
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");

            // Создайте InsertOptions и задайте CopyFormatType
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.SameAsAbove;

            // Вставьте строку с форматированием из вышеуказанного
            worksheet.Cells.InsertRows(2, 1, options);

            // Сохранить результат
            workbook.Save("InsertWithFormatting.xlsx");
        }
    }
}
```

### См. также

* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


