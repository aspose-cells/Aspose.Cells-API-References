---
title: "PivotConditionalFormat.AddCellArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotConditionalFormat. Добавляет область на основе представления сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotconditionalformat/addcellarea/
---
## PivotConditionalFormat.AddCellArea method

Добавляет область на основе представления сводной таблицы.

```csharp
public void AddCellArea(CellArea ca)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | CellArea | Область ячейки. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodAddCellAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 120;
            cells["B3"].Value = 85;
            cells["B4"].Value = 90;

            // Добавьте сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Создайте область ячеек для условного форматирования
            CellArea cellArea = new CellArea();
            cellArea.StartRow = 4;
            cellArea.StartColumn = 5;
            cellArea.EndRow = 6;
            cellArea.EndColumn = 7;

            // Добавьте условное форматирование с областью ячеек
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.AddCellArea(cellArea);

            // Добавить условие форматирования
            int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pcf.FormatConditions[conditionIndex];
            condition.Formula1 = "50";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;

            // Вычислить данные сводной таблицы
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotConditionalFormatWithCellArea.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


