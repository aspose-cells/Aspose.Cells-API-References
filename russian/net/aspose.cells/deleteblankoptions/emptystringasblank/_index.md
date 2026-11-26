---
title: "DeleteBlankOptions.EmptyStringAsBlank"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DeleteBlankOptions. Указывает, будет ли ячейка считаться пустой, когда её значение — пустая строка. Значение по умолчанию: true"
type: docs
url: /ru/net/aspose.cells/deleteblankoptions/emptystringasblank/
---
## DeleteBlankOptions.EmptyStringAsBlank property

Указывает, будет ли ячейка считаться пустой, когда её значение — пустая строка. Значение по умолчанию — true.

```csharp
public bool EmptyStringAsBlank { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyStringAsBlankDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить лист данными, включая пустые строки
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // Настроить DeleteBlankOptions с EmptyStringAsBlank, установленным в true
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true
            };

            // Удалить строки, содержащие пустые строки (рассматриваются как пустые)
            worksheet.Cells.DeleteBlankRows(options);

            // Сохранить результат
            workbook.Save("DeleteBlankOptions_EmptyStringAsBlank_Output.xlsx");
        }
    }
}
```

### См. также

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


