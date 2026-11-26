---
title: "ListColumn.TotalsCalculation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListColumn. Получает и задает тип вычисления в строке Итого столбца списка"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/totalscalculation/
---
## ListColumn.TotalsCalculation property

Получает и задает тип вычисления в строке Totals столбца списка.

```csharp
public TotalsCalculation TotalsCalculation { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyTotalsCalculationDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("Item 3");
            worksheet.Cells["B4"].PutValue(200);

            // Создать объект списка
            int listObjIndex = worksheet.ListObjects.Add(0, 0, 4, 1, true);
            ListObject listObj = worksheet.ListObjects[listObjIndex];
            listObj.ShowTotals = true;
            
            // Установить вычисление итогов для второго столбца
            listObj.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Сохраните книгу
            workbook.Save("ListColumnTotalsCalculationDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TotalsCalculation](../../totalscalculation/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


