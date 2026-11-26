---
title: "PivotTable.ShowInCompactForm"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Оформляет представление сводной таблицы в компактной форме"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showincompactform/
---
## PivotTable.ShowInCompactForm method

Отображает представление сводной таблицы в компактной форме.

```csharp
public void ShowInCompactForm()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInCompactFormDemo
    {
        public static void Run()
        {
            // Создать книгу из исходных данных
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Product");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Electronics");
            sourceSheet.Cells["B2"].PutValue("Laptop");
            sourceSheet.Cells["C2"].PutValue(1200);
            
            sourceSheet.Cells["A3"].PutValue("Electronics");
            sourceSheet.Cells["B3"].PutValue("Phone");
            sourceSheet.Cells["C3"].PutValue(800);
            
            sourceSheet.Cells["A4"].PutValue("Furniture");
            sourceSheet.Cells["B4"].PutValue("Chair");
            sourceSheet.Cells["C4"].PutValue(150);
            
            sourceSheet.Cells["A5"].PutValue("Furniture");
            sourceSheet.Cells["B5"].PutValue("Table");
            sourceSheet.Cells["C5"].PutValue(300);

            // Создать лист со сводной таблицей
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Добавьте сводную таблицу
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("=Sheet1!A1:C5", "A3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Добавить поля в области
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Установить отображение сводной таблицы в компактной форме
            pivotTable.ShowInCompactForm();
            
            // Вычислить данные и обновить
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Сохраните книгу
            workbook.Save("PivotTableCompactFormDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


