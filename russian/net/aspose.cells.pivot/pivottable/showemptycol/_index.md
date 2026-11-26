---
title: "PivotTable.ShowEmptyCol"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, следует ли включать пустые столбцы в таблицу"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showemptycol/
---
## PivotTable.ShowEmptyCol property

Указывает, включать ли пустые столбцы в таблицу.

```csharp
public bool ShowEmptyCol { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyColDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Создайте сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Отобразить текущее значение ShowEmptyCol
            Console.WriteLine("Current ShowEmptyCol value: " + pivotTable.ShowEmptyCol);

            // Установить ShowEmptyCol в false (скрыть пустые столбцы)
            pivotTable.ShowEmptyCol = false;
            Console.WriteLine("ShowEmptyCol set to false - empty columns will be hidden");

            // Вычислить данные сводной таблицы
            pivotTable.CalculateData();

            // Сохранить книгу с скрытыми пустыми столбцами
            workbook.Save("PivotTableHideEmptyCols.xlsx");

            // Установить ShowEmptyCol обратно в true (показать пустые столбцы)
            pivotTable.ShowEmptyCol = true;
            Console.WriteLine("ShowEmptyCol set to true - empty columns will be shown");

            // Повторно вычислить данные сводной таблицы
            pivotTable.CalculateData();

            // Сохранить книгу с видимыми пустыми столбцами
            workbook.Save("PivotTableShowEmptyCols.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


