---
title: "Protection.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Protection. Копировать информацию о защите"
type: docs
url: /ru/net/aspose.cells/protection/copy/
---
## Protection.Copy method

Копировать информацию о защите.

```csharp
public void Copy(Protection source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | Protection |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodCopyWithProtectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте исходные настройки защиты - используйте существующую защиту с листа
            Protection sourceProtection = worksheet.Protection;
            sourceProtection.AllowDeletingColumn = true;
            sourceProtection.AllowInsertingRow = false;
            sourceProtection.Password = "test123";
            sourceProtection.AllowFormattingCell = true;

            // Получить настройки защиты цели
            Protection targetProtection = worksheet.Protection;

            try
            {
                // Вызвать метод Copy с параметром Protection
                targetProtection.Copy(sourceProtection);

                Console.WriteLine("Protection settings copied successfully.");
                Console.WriteLine($"Target protection - AllowDeletingColumn: {targetProtection.AllowDeletingColumn}");
                Console.WriteLine($"Target protection - AllowInsertingRow: {targetProtection.AllowInsertingRow}");
                Console.WriteLine($"Target protection - Password set: {!string.IsNullOrEmpty(targetProtection.Password)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error copying protection settings: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("ProtectionCopyDemo.xlsx");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


