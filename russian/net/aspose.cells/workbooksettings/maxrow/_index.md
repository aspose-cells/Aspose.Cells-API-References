---
title: "WorkbookSettings.MaxRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Возвращает максимальный индекс строки, нумерация с нуля"
type: docs
url: /ru/net/aspose.cells/workbooksettings/maxrow/
---
## WorkbookSettings.MaxRow property

Получает максимальный индекс строки, начиная с нуля.

```csharp
public int MaxRow { get; }
```

### Примечания

Возвращает 65535, если формат файла — Excel97-2003;

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Продемонстрировать свойство MaxRow
            Console.WriteLine("Maximum rows in worksheet: " + workbook.Settings.MaxRow);
            
            // Попробуйте обратиться к ячейке за пределами MaxRow (должно вызвать исключение)
            try
            {
                Cell cell = worksheet.Cells[workbook.Settings.MaxRow + 1, 0];
                Console.WriteLine("This line shouldn't execute");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxRow: " + ex.Message);
            }
            
            // Создайте область ячеек, используя MaxRow
            CellArea area = CellArea.CreateCellArea(0, 0, workbook.Settings.MaxRow, 0);
            Console.WriteLine("Created cell area from row 0 to MaxRow: " + area.EndRow);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


