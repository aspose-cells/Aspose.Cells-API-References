---
title: "Класс AbstractFormulaChangeMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.AbstractFormulaChangeMonitor. Монитор для отслеживания пользователем изменений формул во время определённых операций"
type: docs
url: /ru/net/aspose.cells/abstractformulachangemonitor/
---
## AbstractFormulaChangeMonitor class

Мониторинг для пользователя, позволяющий отслеживать изменения формул во время определённых операций.

```csharp
public abstract class AbstractFormulaChangeMonitor
```

## Методы

| Имя | Описание |
| --- | --- |
| virtual [OnCellFormulaChanged](../../aspose.cells/abstractformulachangemonitor/oncellformulachanged/)(int, int, int) | Событие, которое будет вызвано при изменении формулы в ячейке. |
| virtual [OnFormatConditionFormulaChanged](../../aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/)(FormatCondition) | Событие, которое будет вызвано при изменении формулы FormatCondition. |

### Примечания

Например, при удалении/вставке диапазона ячеек формулы других ячеек могут измениться из‑за сдвига ссылок. Обратите внимание, что методы в мониторе могут вызываться несколько раз для одного объекта, содержащего формулу.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassAbstractFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Установите несколько формул в ячейках
            worksheet.Cells["A1"].Formula = "=B1+C1";
            worksheet.Cells["B1"].Formula = "=D1*2";
            worksheet.Cells["C1"].Value = 5;
            worksheet.Cells["D1"].Value = 10;

            InsertOptions options = new InsertOptions();
            options.FormulaChangeMonitor = new MyFormulaChangeMonitor(wb.Worksheets);
            
            // Вставьте строки, которые вызовут изменения формул
            worksheet.Cells.InsertRows(0, 2, options);
        }
    }

    public class MyFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        private readonly WorksheetCollection mWorksheets;
        
        public MyFormulaChangeMonitor(WorksheetCollection worksheets)
        {
            mWorksheets = worksheets;
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"Formula changed in {mWorksheets[sheetIndex].Name}!{CellsHelper.CellIndexToName(rowIndex, columnIndex)}");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


