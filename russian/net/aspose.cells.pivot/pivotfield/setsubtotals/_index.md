---
title: "PivotField.SetSubtotals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Устанавливает способ подсчёта итогов для указанного поля"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/setsubtotals/
---
## PivotField.SetSubtotals method

Устанавливает, как подсчитывать промежуточный итог указанного поля.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | [`PivotFieldSubtotalType`](../../pivotfieldsubtotaltype/) |
| показано | Boolean | Указывает, отображает ли указанное поле итоги. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            var cells = sheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = "TV";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Electronics";
            cells["B3"].Value = "Radio";
            cells["C3"].Value = 500;
            
            cells["A4"].Value = "Clothing";
            cells["B4"].Value = "Shirt";
            cells["C4"].Value = 300;
            
            cells["A5"].Value = "Clothing";
            cells["B5"].Value = "Pants";
            cells["C5"].Value = 400;

            // Добавьте сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Добавить поля строк
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // Продемонстрировать SetSubtotals с PivotFieldSubtotalType и логическим значением
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotFieldSetSubtotalsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


