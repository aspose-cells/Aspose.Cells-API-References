---
title: "Protection.AllowDeletingRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Указывает, разрешено ли удаление строк на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowdeletingrow/
---
## Protection.AllowDeletingRow property

Представляет, разрешено ли удаление строк на защищённом листе.

```csharp
public bool AllowDeletingRow { get; set; }
```

### Примечания

Строки, содержащие ячейки, которые нужно удалить, должны быть разблокированы, когда лист защищён, и опция "Select unlocked cells" должна быть включена.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Установите параметры защиты
            Protection protection = sheet.Protection;
            protection.AllowDeletingRow = true;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingColumn = true;

            // Защитить лист
            sheet.Protect(ProtectionType.All);

            // Сохраните книгу
            workbook.Save("output.xlsx");

            // Загрузить сохранённую книгу для проверки настроек
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            // Проверьте AllowDeletingRow и другие свойства
            Console.WriteLine("AllowDeletingRow: " + loadedSheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowSorting: " + loadedSheet.Protection.AllowSorting);
            Console.WriteLine("AllowFiltering: " + loadedSheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingColumn: " + loadedSheet.Protection.AllowFormattingColumn);
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


