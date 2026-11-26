---
title: "Cell.IsInTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Указывает, является ли эта ячейка частью табличной формулы"
type: docs
url: /ru/net/aspose.cells/cell/isintable/
---
## Cell.IsInTable property

Указывает, является ли эта ячейка частью формулы таблицы.

```csharp
[Obsolete("Use IsTableFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInTable { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте Cell.IsTableFormula, чтобы проверить, является ли формула ячейки частью табличной формулы. Это свойство будет удалено через 12 месяцев, начиная с мая 2018 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellPropertyIsInTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);

            // Создать таблицу из диапазона данных
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            try
            {
                // Проверьте свойство IsInTable для ячеек внутри и вне таблицы
                Cell cellInTable = worksheet.Cells["A2"];
                Cell cellOutsideTable = worksheet.Cells["C2"];

                Console.WriteLine("Cell A2 (inside table):");
                Console.WriteLine("  Value: " + cellInTable.StringValue);
                Console.WriteLine("  IsInTable: " + cellInTable.IsInTable);

                Console.WriteLine("\nCell C2 (outside table):");
                Console.WriteLine("  Value: " + cellOutsideTable.StringValue);
                Console.WriteLine("  IsInTable: " + cellOutsideTable.IsInTable);

                // Сохраните книгу
                workbook.Save("IsInTableDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


