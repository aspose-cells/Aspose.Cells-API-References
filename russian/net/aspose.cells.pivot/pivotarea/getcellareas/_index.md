---
title: "PivotArea.GetCellAreas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotArea. Получает области ячеек этой области сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotarea/getcellareas/
---
## PivotArea.GetCellAreas method

Получает области ячеек этого сводного диапазона.

```csharp
public CellArea[] GetCellAreas()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaMethodGetCellAreasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать минимальные данные сводной таблицы
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";

            try
            {
                // Создать сводную таблицу с базовой конфигурацией
                int pivotIndex = worksheet.PivotTables.Add("A1:A3", "D1", "DemoPivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Инициализировать область сводной таблицы с экземпляром PivotTable
                PivotArea pivotArea = new PivotArea(pivotTable);

                // Настроить параметры области сводной таблицы
                pivotArea.RuleType = PivotAreaType.Normal;
                pivotArea.AxisType = PivotFieldType.Data;
                pivotArea.IsRowGrandIncluded = true;

                // Выполнить целевой метод
                CellArea[] cellAreas = pivotArea.GetCellAreas();

                Console.WriteLine($"GetCellAreas returned {cellAreas.Length} cell area(s)");
                foreach (CellArea area in cellAreas)
                {
                    Console.WriteLine($"CellArea: Columns {area.StartColumn}-{area.EndColumn}, Rows {area.StartRow}-{area.EndRow}");
                }

                workbook.Save("GetCellAreasDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetCellAreas: {ex.Message}");
            }
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


