---
title: "PivotField.GetFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Получает формулу вычисляемого поля. Работает только с вычисляемыми полями"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/getformula/
---
## PivotField.GetFormula method

Получает формулу вычисляемого поля. Работает только для вычисляемого поля.

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
    public class PivotFieldMethodGetFormulaDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;
            
            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить вычисляемое поле с формулой
            pivotTable.AddCalculatedField("=ABS('Sales')", "Absolute Sales");
            
            // Получить формулу из вычисляемого поля
            PivotFieldCollection fields = pivotTable.DataFields;
            string formula = fields[fields.Count - 1].GetFormula();
            
            // Вывести формулу
            Console.WriteLine("Calculated field formula: " + formula);
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


