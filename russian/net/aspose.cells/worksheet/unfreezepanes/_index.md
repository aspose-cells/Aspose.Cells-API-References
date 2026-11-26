---
title: "Worksheet.UnFreezePanes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Размораживает области листа"
type: docs
url: /ru/net/aspose.cells/worksheet/unfreezepanes/
---
## Worksheet.UnFreezePanes method

Размораживает области в листе.

```csharp
public void UnFreezePanes()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnFreezePanesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Заморозить области в ячейке C3 (заморожены строки 2, столбцы 2)
            worksheet.FreezePanes("C3", 2, 2);

            // Проверьте, что области заморожены
            int frozenRow, frozenColumn, frozenRows, frozenColumns;
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"Frozen panes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Разморозить области
            worksheet.UnFreezePanes();

            // Проверьте, что области разморожены
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"After UnFreezePanes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Сохраните книгу
            workbook.Save("UnFreezePanesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


