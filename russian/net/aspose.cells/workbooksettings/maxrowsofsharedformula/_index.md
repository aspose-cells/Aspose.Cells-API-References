---
title: "WorkbookSettings.MaxRowsOfSharedFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает и задает максимальный номер строки совместной формулы"
type: docs
url: /ru/net/aspose.cells/workbooksettings/maxrowsofsharedformula/
---
## WorkbookSettings.MaxRowsOfSharedFormula property

Получает и задает максимальный номер строки общей формулы.

```csharp
public int MaxRowsOfSharedFormula { get; set; }
```

### Примечания

Если число слишком велико, автoфильтр работает очень медленно в MS Excel 2013.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowsOfSharedFormulaDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            book.Settings.MaxRowsOfSharedFormula = 100;
            
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Установить общую формулу с 101 строкой (превышает MaxRowsOfSharedFormula)
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            // Проверьте формулу в последней ячейке
            Console.WriteLine("Formula in B101: " + cells["B101"].Formula);
            
            // Увеличьте MaxRowsOfSharedFormula и снова протестируйте на новом листе
            book.Settings.MaxRowsOfSharedFormula = 1024;
            Worksheet sheet2 = book.Worksheets.Add("Sheet2");
            cells = sheet2.Cells;
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            Console.WriteLine("Formula in B101 (Sheet2): " + cells["B101"].Formula);
            
            book.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


