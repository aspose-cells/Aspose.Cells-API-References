---
title: "FormatConditionCollection.AddArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FormatConditionCollection. Добавляет диапазон ячеек с условным форматированием"
type: docs
url: /ru/net/aspose.cells/formatconditioncollection/addarea/
---
## FormatConditionCollection.AddArea method

Добавляет условно отформатированный диапазон ячеек.

```csharp
public int AddArea(CellArea cellArea)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | CellArea | Диапазон ячеек с условным форматированием. |

### Возвращаемое значение

Индекс диапазона ячеек с условным форматированием.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue(row * col);
                }
            }

            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection formatCollection = worksheet.ConditionalFormattings[index];
            
            // Создайте условие форматирования.
            formatCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Создать области ячеек и добавить их в коллекцию форматов
            CellArea area1 = CellArea.CreateCellArea(0, 0, 4, 4);
            CellArea area2 = CellArea.CreateCellArea(5, 5, 9, 9);
            
            formatCollection.AddArea(area1);
            formatCollection.AddArea(area2);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


