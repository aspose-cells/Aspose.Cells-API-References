---
title: "PivotField.BaseIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Представляет индекс в исходных полях сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/baseindex/
---
## PivotField.BaseIndex property

Представляет индекс в исходных полях сводной таблицы.

```csharp
public int BaseIndex { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот сеттер свойства теперь устарел. Этот сеттер будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyBaseIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = "PivotData";
            
            // Пример данных
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["B1"].PutValue("Quarter");
            ws.Cells["C1"].PutValue("Sales");
            
            ws.Cells["A2"].PutValue("Electronics");
            ws.Cells["A3"].PutValue("Electronics");
            ws.Cells["A4"].PutValue("Clothing");
            ws.Cells["A5"].PutValue("Clothing");
            
            ws.Cells["B2"].PutValue("Q1");
            ws.Cells["B3"].PutValue("Q2");
            ws.Cells["B4"].PutValue("Q1");
            ws.Cells["B5"].PutValue("Q2");
            
            ws.Cells["C2"].PutValue(1000);
            ws.Cells["C3"].PutValue(1200);
            ws.Cells["C4"].PutValue(800);
            ws.Cells["C5"].PutValue(900);

            // Создать сводную таблицу — исправлено получением PivotTable по индексу
            int pivotIndex = ws.PivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pt = ws.PivotTables[pivotIndex];
            
            // Добавить поле строки
            int rowIndex = pt.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pt.RowFields[rowIndex];
            
            // Добавить поле столбца (будет использоваться как базовое поле)
            int colIndex = pt.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField quarterField = pt.ColumnFields[colIndex];
            
            // Добавить поле данных с обычным расчётом
            int dataIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pt.DataFields[dataIndex];
            dataField.Function = ConsolidationFunction.Sum;
            
            // Добавить второе поле данных, показывающее разницу с предыдущим кварталом
            int diffIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField diffField = pt.DataFields[diffIndex];
            diffField.DisplayName = "QoQ Difference";
            diffField.ShowValuesAs(
                PivotFieldDataDisplayFormat.DifferenceFrom, 
                quarterField.BaseIndex, 
                PivotItemPositionType.Previous,
                0);
            
            // Выполнить расчёт и сохранить
            wb.CalculateFormula();
            wb.Save("PivotTableWithBaseIndexDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


