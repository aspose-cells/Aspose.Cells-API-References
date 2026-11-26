---
title: "PivotTable.ColumnGrand"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, отображает ли отчет сводной таблицы общие итоги по столбцам"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/columngrand/
---
## PivotTable.ColumnGrand property

Указывает, отображает ли отчет сводной таблицы общие итоги по столбцам.

```csharp
[Obsolete("Use PivotTable.ShowColumnGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ColumnGrand { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте метод PivotTable.ShowColumnGrandTotals. Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Компания Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyColumnGrandDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Отобразить текущее значение ColumnGrand
            Console.WriteLine("Current ColumnGrand value: " + pivotTable.ColumnGrand);

            // Изменить свойство ColumnGrand
            pivotTable.ColumnGrand = false;

            // Вычислить данные, чтобы увидеть эффект
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotTableColumnGrandDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


