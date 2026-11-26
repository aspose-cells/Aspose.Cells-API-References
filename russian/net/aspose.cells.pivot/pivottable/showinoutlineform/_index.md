---
title: "PivotTable.ShowInOutlineForm"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Размещает PivotTable в виде схемы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showinoutlineform/
---
## PivotTable.ShowInOutlineForm method

Отображает сводную таблицу в виде схемы.

```csharp
public void ShowInOutlineForm()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInOutlineFormDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист с образцовыми данными
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Добавьте примерные данные
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["B1"].PutValue("Product");
            dataSheet.Cells["C1"].PutValue("Sales");
            
            dataSheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            dataSheet.Cells["B2"].PutValue("Apple");
            dataSheet.Cells["C2"].PutValue(1000);
            
            dataSheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2));
            dataSheet.Cells["B3"].PutValue("Banana");
            dataSheet.Cells["C3"].PutValue(2000);
            
            dataSheet.Cells["A4"].PutValue(new DateTime(2023, 1, 3));
            dataSheet.Cells["B4"].PutValue("Apple");
            dataSheet.Cells["C4"].PutValue(1500);
            
            // Создать лист сводной таблицы
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Добавить сводную таблицу и получить ссылку
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C4", 
                "A3", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
                
            // Добавить поля в области
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Показать в виде схемы
            pivotTable.ShowInOutlineForm();
            
            // Обновить и вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotTableOutlineFormDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


