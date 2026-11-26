---
title: "ListColumn.IsArrayFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListColumn. Указывает, является ли формула массивной формулой"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/isarrayformula/
---
## ListColumn.IsArrayFormula property

Указывает, является ли формула массивной.

```csharp
public bool IsArrayFormula { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для создания таблицы
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);

            // Создать объект таблицы/списка
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[tableIndex];

            // Добавить массивную формулу во второй столбец
            listObject.ListColumns[1].Formula = "{=SUM(A2:A3*B2:B3)}";

            try
            {
                // Получить доступ к свойству IsArrayFormula (только для чтения)
                bool isArrayFormula = listObject.ListColumns[1].IsArrayFormula;

                // Отобразить значение
                Console.WriteLine("IsArrayFormula value: " + isArrayFormula);

                // Сохраните книгу
                workbook.Save("IsArrayFormulaDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


