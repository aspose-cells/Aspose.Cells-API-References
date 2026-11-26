---
title: "AbstractFormulaChangeMonitor.OnCellFormulaChanged"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractFormulaChangeMonitor. Событие, которое будет вызвано, когда формула в ячейке изменяется."
type: docs
url: /ru/net/aspose.cells/abstractformulachangemonitor/oncellformulachanged/
---
## AbstractFormulaChangeMonitor.OnCellFormulaChanged method

Событие, которое будет вызвано при изменении формулы в ячейке.

```csharp
public virtual void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | Int32 | Индекс листа изменённой ячейки. |
| rowIndex | Int32 | Индекс строки изменённой ячейки. |
| columnIndex | Int32 | Индекс столбца изменённой ячейки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo : AbstractFormulaChangeMonitor
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр нашего демонстрационного класса, наследующего AbstractFormulaChangeMonitor.
            var monitor = new AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo();

            // Установите формулу в ячейке, чтобы вызвать изменение.
            worksheet.Cells["A1"].Formula = "=SUM(B1:B10)";

            try
            {
                // Вызовите OnCellFormulaChanged с индексом листа 0, строки 0, столбца 0 (A1).
                monitor.OnCellFormulaChanged(0, 0, 0);

                Console.WriteLine("OnCellFormulaChanged called successfully for cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnCellFormulaChanged method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("OnCellFormulaChangedDemo.xlsx");
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            // Реализация обработки изменения формулы.
            Console.WriteLine($"Formula changed in sheet {sheetIndex} at row {rowIndex}, column {columnIndex}");
        }

    }
}
```

### См. также

* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


