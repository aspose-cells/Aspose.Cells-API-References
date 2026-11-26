---
title: "PivotConditionalFormat.ApplyTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotConditionalFormat. Применяет условное форматирование к диапазону, который должен находиться в области данных"
type: docs
url: /ru/net/aspose.cells.pivot/pivotconditionalformat/applyto/
---
## PivotConditionalFormat.ApplyTo method

Применяет условное форматирование к диапазону, который должен находиться в области данных.

```csharp
public void ApplyTo(int row, int column, PivotConditionFormatScopeType scope)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Выбранная строка. |
| column | Int32 | Выбранный столбец. |
| область | PivotConditionFormatScopeType | Область |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodApplyToWithInt32Int32PivotConditionFormatDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Добавьте сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotTableIndex = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotTableIndex];
            
            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Добавить условный формат
            PivotConditionalFormatCollection pcfCollection = pivotTable.ConditionalFormats;
            PivotConditionalFormat pcf = pcfCollection[pcfCollection.Add()];
            
            // Продемонстрировать метод ApplyTo с конкретными параметрами
            pcf.ApplyTo(0, 1, PivotConditionFormatScopeType.Field);
            
            // Добавить условие форматирования
            FormatConditionCollection fcc = pcf.FormatConditions;
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "20";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = System.Drawing.Color.LightGreen;
            
            // Вычислите данные и сохраните
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatApplyToDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


