---
title: "PivotTable.SelectArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Выберите область представления сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/selectarea/
---
## PivotTable.SelectArea method

Выберите область представления сводной таблицы.

```csharp
public PivotAreaCollection SelectArea(CellArea ca)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | CellArea | Область ячейки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodSelectAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Вычислить данные
            pivotTable.CalculateData();

            // Определите область ячейки для выбора
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 5;
            area.EndColumn = 6;

            try
            {
                // Вызовите метод SelectArea с параметром CellArea
                PivotAreaCollection selectedAreas = pivotTable.SelectArea(area);
                
                Console.WriteLine("SelectArea method executed successfully. Selected areas count: " + selectedAreas.Count);
                
                // Сохраните книгу, чтобы показать эффект
                workbook.Save("PivotTableSelectAreaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SelectArea method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotAreaCollection](../../pivotareacollection/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


