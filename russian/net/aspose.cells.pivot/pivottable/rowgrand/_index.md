---
title: "PivotTable.RowGrand"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, следует ли показывать общие итоги для строк этой сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/rowgrand/
---
## PivotTable.RowGrand property

Указывает, следует ли показывать общие итоги для строк этой сводной таблицы.

```csharp
[Obsolete("Use PivotTable.ShowRowGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool RowGrand { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте метод PivotTable.ShowRowGrandTotals. Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyRowGrandDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);
            
            worksheet.Cells["A5"].PutValue("Product A");
            worksheet.Cells["B5"].PutValue("West");
            worksheet.Cells["C5"].PutValue(1500);
            
            worksheet.Cells["A6"].PutValue("Product B");
            worksheet.Cells["B6"].PutValue("North");
            worksheet.Cells["C6"].PutValue(2500);

            // Создайте сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C6", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Отобразить текущее значение RowGrand
            Console.WriteLine("Current RowGrand value: " + pivotTable.RowGrand);

            // Изменить свойство RowGrand
            pivotTable.RowGrand = false;

            // Вычислить данные сводной таблицы
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotTablePropertyRowGrandDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


