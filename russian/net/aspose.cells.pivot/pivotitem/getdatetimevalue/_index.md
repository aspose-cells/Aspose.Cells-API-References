---
title: "PivotItem.GetDateTimeValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotItem. Получает значение даты и времени элемента сводной таблицы. Если значение равно null, будет возвращено DateTime.MinValue"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/getdatetimevalue/
---
## PivotItem.GetDateTimeValue method

Получает значение даты и времени элемента сводки. Если значение равно null, будет возвращено DateTime.MinValue

```csharp
public DateTime GetDateTimeValue()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetDateTimeValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные со значением даты
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            worksheet.Cells["A3"].PutValue(DateTime.Now);
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            foreach (PivotItem pivotItem in pivotItems)
            {
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();
                Console.WriteLine("DateTime Value: " + dateTimeValue);
            }

            workbook.Save("PivotItemGetDateTimeValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


