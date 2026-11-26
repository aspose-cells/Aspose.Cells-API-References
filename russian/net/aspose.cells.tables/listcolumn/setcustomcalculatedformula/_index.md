---
title: "ListColumn.SetCustomCalculatedFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListColumn. Устанавливает формулу для этого столбца списка"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/setcustomcalculatedformula/
---
## ListColumn.SetCustomCalculatedFormula method

Устанавливает формулу для этого столбца списка.

```csharp
public void SetCustomCalculatedFormula(string formula, bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | формула для этого столбца списка. |
| isR1C1 | Boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | Boolean | Нужно ли форматировать формулу в соответствии с локалью. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnMethodSetCustomCalculatedFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Total");

            // Создайте таблицу
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true); // Adjusted parameters to match correct overload
            ListObject table = worksheet.ListObjects[tableIndex];

            // Получить второй столбец списка
            ListColumn totalColumn = table.ListColumns[1];

            try
            {
                // Установить пользовательскую формулу, используя нотацию A1 со стандартной локалью
                totalColumn.SetCustomCalculatedFormula("=A2*1.1", false, false);
                
                Console.WriteLine("Custom formula set successfully.");
                Console.WriteLine($"Cell B2 formula: {worksheet.Cells["B2"].Formula}");
                Console.WriteLine($"Cell B3 formula: {worksheet.Cells["B3"].Formula}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("SetCustomCalculatedFormulaExample.xlsx");
        }
    }
}
```

### См. также

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


