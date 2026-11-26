---
title: "SpreadsheetML2003SaveOptions.LimitAsXls"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SpreadsheetML2003SaveOptions. При ограничении как xls максимальный индекс строки — 65535, а максимальный индекс столбца — 255."
type: docs
url: /ru/net/aspose.cells/spreadsheetml2003saveoptions/limitasxls/
---
## SpreadsheetML2003SaveOptions.LimitAsXls property

Ограничение как в xls: максимальный индекс строки — 65535, а максимальный индекс столбца — 255.

```csharp
public bool LimitAsXls { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyLimitAsXlsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Получите доступ к ячейкам и создайте диапазон.
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "C5");
            range.Name = "TestRange";
            
            // Сохраните с LimitAsXls = true.
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
            {
                LimitAsXls = true
            };
            
            // Сохраните как SpreadsheetML с ограничениями XLS.
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with LimitAsXls=true");
        }
    }
}
```

### См. также

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


