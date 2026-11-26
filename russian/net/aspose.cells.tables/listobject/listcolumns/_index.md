---
title: "ListObject.ListColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Получает список ListColumn этой таблицы"
type: docs
url: /ru/net/aspose.cells.tables/listobject/listcolumns/
---
## ListObject.ListColumns property

Получает список [`ListColumn`](../../listcolumn/) этой таблицы.

```csharp
public ListColumnCollection ListColumns { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyListColumnsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Создать объект списка
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add(0, 0, 9, 4, true);
            ListObject listObject = listObjects[index];
            
            // Включить итоги и задать вычисление для 5-го столбца
            listObject.ShowTotals = true;
            listObject.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
            
            // Применить стиль таблицы
            listObject.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleLight4;

            // Сохраните книгу
            workbook.Save("ListColumnsDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [ListColumnCollection](../../listcolumncollection/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


