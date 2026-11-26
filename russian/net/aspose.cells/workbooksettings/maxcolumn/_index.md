---
title: "WorkbookSettings.MaxColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает максимальный индекс столбца, начиная с нуля"
type: docs
url: /ru/net/aspose.cells/workbooksettings/maxcolumn/
---
## WorkbookSettings.MaxColumn property

Получает максимальный индекс столбца, начиная с нуля.

```csharp
public int MaxColumn { get; }
```

### Примечания

Возвращает 255, если формат файла Excel97-2003;

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Console.WriteLine("MaxColumn value: " + workbook.Settings.MaxColumn);
            
            // Продемонстрировать использование MaxColumn, попытавшись обратиться к столбцу за пределами ограничения
            try
            {
                Cells cells = workbook.Worksheets[0].Cells;
                Cell cell = cells[0, workbook.Settings.MaxColumn + 1];
                Console.WriteLine("This should not be reached");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxColumn: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


