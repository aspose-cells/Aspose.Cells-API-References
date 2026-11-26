---
title: "PivotTable.ConditionalFormats"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Получает условные форматы сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/conditionalformats/
---
## PivotTable.ConditionalFormats property

Получает условные форматы сводной таблицы.

```csharp
public PivotConditionalFormatCollection ConditionalFormats { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyConditionalFormatsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 120;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 85;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 95;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 110;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Добавьте строки и поля данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Добавить условный формат
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.AddFieldArea(PivotFieldType.Data, pivotTable.DataFields[0]);
            
            // Добавить условие форматирования
            int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pcf.FormatConditions[conditionIndex];
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Formula1 = "100";
            condition.Style.BackgroundColor = Color.Red;

            // Сохранить книгу
            workbook.Save("PivotTableConditionalFormatting.xlsx");
        }
    }
}
```

### См. также

* class [PivotConditionalFormatCollection](../../pivotconditionalformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


