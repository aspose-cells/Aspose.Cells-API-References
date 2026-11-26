---
title: "PivotTable.ShowInTabularForm"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Форматирует PivotTable в табличной форме"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showintabularform/
---
## PivotTable.ShowInTabularForm method

Отображает сводную таблицу в табличной форме.

```csharp
public void ShowInTabularForm()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInTabularFormDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист данных
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Добавить примерные данные для сводной таблицы
            dataSheet.Cells["A1"].PutValue("Label");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);

            // Добавить лист pivot table
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Добавьте сводную таблицу
            int pivotIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Добавить поля в сводную таблицу
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Отобразить pivot table в табличной форме
            pivotTable.ShowInTabularForm();
            
            // Обновить и вычислить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotTableShowInTabularFormDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


