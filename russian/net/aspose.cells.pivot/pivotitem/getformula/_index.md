---
title: "PivotItem.GetFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotItem. Получает формулу этого вычисляемого элемента. Работает только когда элемент является вычисляемым"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/getformula/
---
## PivotItem.GetFormula method

Получает формулу этого вычисляемого элемента. Работает только когда элемент является вычисляемым.

```csharp
public string GetFormula()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetFormulaDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Добавить сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Получить формулу из элементов сводной таблицы
            string rowItemFormula = pivotTable.RowFields[0].PivotItems[0].GetFormula();
            string dataFieldFormula = pivotTable.DataFields[0].GetFormula();

            Console.WriteLine("Row Item Formula: " + rowItemFormula);
            Console.WriteLine("Data Field Formula: " + dataFieldFormula);
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


