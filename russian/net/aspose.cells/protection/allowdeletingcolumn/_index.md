---
title: "Protection.AllowDeletingColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Описывает, разрешено ли удалять столбцы на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowdeletingcolumn/
---
## Protection.AllowDeletingColumn property

Представляет, разрешено ли удаление столбцов на защищённом листе.

```csharp
public bool AllowDeletingColumn { get; set; }
```

### Примечания

Столбцы, содержащие удаляемые ячейки, должны быть разблокированы при защите листа, и опция "Select unlocked cells" должна быть включена.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Включить защиту листа
            Protection protection = worksheet.Protection;
            protection.AllowDeletingColumn = true;
            worksheet.Protect(ProtectionType.All);

            // Проверьте настройку
            Console.WriteLine("AllowDeletingColumn: " + protection.AllowDeletingColumn);

            // Попробуйте удалить столбец (должно работать, так как AllowDeletingColumn равно true)
            worksheet.Cells.DeleteColumn(0);
            Console.WriteLine("Column deleted successfully");

            // Отключить удаление столбцов
            protection.AllowDeletingColumn = false;

            // Попробуйте удалить другой столбец (должно завершиться ошибкой)
            try
            {
                worksheet.Cells.DeleteColumn(1);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Failed to delete column: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


