---
title: "DeleteOptions.FormulaChangeMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DeleteOptions. Получает/устанавливает монитор для отслеживания изменений, вызванных удалением"
type: docs
url: /ru/net/aspose.cells/deleteoptions/formulachangemonitor/
---
## DeleteOptions.FormulaChangeMonitor property

Получает/задает монитор для отслеживания изменений, вызванных удалением.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Подготовьте тестовые данные
            cells["A1"].Formula = "=A5";
            cells["A5"].Value = 10;
            
            // Добавить условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            fcc.Add(CellArea.CreateCellArea(0, 3, 1, 4), FormatConditionType.Expression,
                OperatorType.Equal, "=A8>0", "");

            // Создайте и назначьте монитор
            CustomFormulaChangeMonitor monitor = new CustomFormulaChangeMonitor();
            DeleteOptions options = new DeleteOptions
            {
                FormulaChangeMonitor = monitor,
                UpdateReference = true
            };

            // Удалите строку, которая должна вызвать изменения формул
            cells.DeleteRows(2, 1, options);

            // Выведите результаты мониторинга
            Console.WriteLine("Cell formula changes detected: " + monitor.CellChangesDetected);
            Console.WriteLine("Format condition changes detected: " + monitor.FormatConditionChangesDetected);
        }
    }

    public class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        public bool CellChangesDetected { get; private set; }
        public bool FormatConditionChangesDetected { get; private set; }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            CellChangesDetected = true;
            Console.WriteLine($"Cell formula changed at Sheet {sheetIndex}, Row {rowIndex}, Column {columnIndex}");
        }

        public override void OnFormatConditionFormulaChanged(FormatCondition fc)
        {
            FormatConditionChangesDetected = true;
            Console.WriteLine("Format condition formula changed");
        }
    }
}
```

### См. также

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


