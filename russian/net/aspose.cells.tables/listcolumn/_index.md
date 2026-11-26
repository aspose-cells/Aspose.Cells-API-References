---
title: "Класс ListColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Tables.ListColumn. Представляет столбец в таблице"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/
---
## ListColumn class

Представляет столбец в таблице.

```csharp
public class ListColumn
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Formula](../../aspose.cells.tables/listcolumn/formula/) { get; set; } | Получает и задает формулу столбца списка. |
| [IsArrayFormula](../../aspose.cells.tables/listcolumn/isarrayformula/) { get; } | Указывает, является ли формула массивной. |
| [Name](../../aspose.cells.tables/listcolumn/name/) { get; set; } | Получает и задает имя столбца. |
| [Range](../../aspose.cells.tables/listcolumn/range/) { get; } | Получает диапазон этого столбца списка. |
| [TotalsCalculation](../../aspose.cells.tables/listcolumn/totalscalculation/) { get; set; } | Получает и задает тип вычисления в строке Totals столбца списка. |
| [TotalsRowLabel](../../aspose.cells.tables/listcolumn/totalsrowlabel/) { get; set; } | Получает и задает отображаемые метки строки итогов. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/getcustomcalculatedformula/)(bool, bool) | Получает формулу этого столбца списка. |
| [GetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/getcustomtotalsrowformula/)(bool, bool) | Получает формулу строки итогов этого столбца списка. |
| [GetDataStyle](../../aspose.cells.tables/listcolumn/getdatastyle/)() | Получает стиль данных в этом столбце таблицы. |
| [SetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/setcustomcalculatedformula/)(string, bool, bool) | Устанавливает формулу для этого столбца списка. |
| [SetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/setcustomtotalsrowformula/)(string, bool, bool) | Получает формулу строки итогов этого столбца списка. |
| [SetDataStyle](../../aspose.cells.tables/listcolumn/setdatastyle/)(Style) | Устанавливает стиль данных в этом столбце таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnDemo
    {
        public static void ListColumnExample()
        {
            // Создать новую книгу и получить доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполните лист некоторыми данными
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 4; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Добавить объект ListObject (таблицу) в лист
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];
            table.ShowTotals = true;

            // Получить доступ к ListColumn и установить его свойства
            ListColumn listColumn = table.ListColumns[4];
            listColumn.TotalsCalculation = TotalsCalculation.Sum;
            listColumn.Formula = "=[A]";
            listColumn.Name = "CustomColumn";
            listColumn.TotalsRowLabel = "Total";

            // Сохраните книгу
            workbook.Save("ListColumnExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


