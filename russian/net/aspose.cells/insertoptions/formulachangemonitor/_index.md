---
title: "InsertOptions.FormulaChangeMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство InsertOptions. Получает/устанавливает монитор для отслеживания изменений, вызванных вставкой"
type: docs
url: /ru/net/aspose.cells/insertoptions/formulachangemonitor/
---
## InsertOptions.FormulaChangeMonitor property

Получает/задаёт монитор для отслеживания изменений, вызванных вставкой.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsPropertyFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые примерные данные с формулами
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Formula = "=A1*2";
            worksheet.Cells["B1"].Formula = "=SUM(A1:A2)";

            try
            {
                // Создайте экземпляр InsertOptions
                InsertOptions options = new InsertOptions();

                // Создайте пользовательскую реализацию FormulaChangeMonitor
                var monitor = new CustomFormulaChangeMonitor();
                options.FormulaChangeMonitor = monitor;

                // Отобразите текущий FormulaChangeMonitor
                Console.WriteLine("FormulaChangeMonitor is set: " +
                    (options.FormulaChangeMonitor != null));

                // Вставьте строки, которые могут вызвать изменения формул
                worksheet.Cells.InsertRows(1, 1, options);

                // Сохранить результат
                workbook.Save("FormulaChangeMonitorDemo.xlsx");
                Console.WriteLine("FormulaChangeMonitor demonstration completed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Пользовательская реализация AbstractFormulaChangeMonitor
        private class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
        {
            public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
            {
                Console.WriteLine($"Formula changed at Sheet {sheetIndex}, Cell {rowIndex},{columnIndex}");
            }

            public override void OnFormatConditionFormulaChanged(FormatCondition fc)
            {
                Console.WriteLine($"Format condition formula changed: {fc.Formula1}");
            }
        }
    }
}
```

### См. также

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


