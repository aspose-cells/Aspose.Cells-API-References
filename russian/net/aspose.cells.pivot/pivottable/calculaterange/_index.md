---
title: "PivotTable.CalculateRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Вычисляет диапазон сводных таблиц"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/calculaterange/
---
## PivotTable.CalculateRange method

Вычисляет диапазон сводной таблицы.

```csharp
public void CalculateRange()
```

### Примечания

Если этот метод не был вызван, возможно диапазон сводной таблицы некорректен.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте примерные данные в первый лист
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["B2"].PutValue(1000);
            dataSheet.Cells["A3"].PutValue("Banana");
            dataSheet.Cells["B3"].PutValue(2000);
            dataSheet.Cells["A4"].PutValue("Orange");
            dataSheet.Cells["B4"].PutValue(3000);

            // Добавить сводную таблицу
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("A1", "A1:B4", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Добавьте строки и поля данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Вычислить диапазон и обновить данные
            pivotTable.CalculateRange();
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Сохраните книгу
            workbook.Save("PivotTableCalculateRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


