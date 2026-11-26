---
title: "DeleteBlankOptions.EmptyFormulaValueAsBlank"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DeleteBlankOptions. Будет ли ячейка считаться пустой, если она содержит формулу, а вычисленный результат равен null или пустой строке. Значение по умолчанию: false"
type: docs
url: /ru/net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

Будет ли ячейка считаться пустой, если она содержит формулу, а вычисленный результат равен null или пустой строке. Значение по умолчанию — false.

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### Примечания

Как правило, пользователь должен убедиться, что формулы вычислены до операции удаления, когда это свойство установлено в true. В противном случае все недавно созданные формулы обычными API, такими как [`Formula`](../../cell/formula/), будут считаться пустыми и могут быть удалены, поскольку до вычисления их результаты равны null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyFormulaValueAsBlankDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Заполнить примерными данными
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";  // Formula returning blank
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1"; // Formula with value
            
            // Удалить пустые строки, не учитывая пустые формулы
            Console.WriteLine("Before deletion (normal): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows();
            Console.WriteLine("After normal deletion: " + cells.MaxRow + " rows");

            // Сбросить данные
            cells.ClearContents(0, 0, cells.MaxRow + 1, cells.MaxColumn + 1);
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1";

            // Удалить пустые строки, рассматривая пустые формулы как пустые
            Console.WriteLine("\nBefore deletion (with EmptyFormulaValueAsBlank): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            Console.WriteLine("After deletion with EmptyFormulaValueAsBlank: " + cells.MaxRow + " rows");
        }
    }
}
```

### См. также

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


