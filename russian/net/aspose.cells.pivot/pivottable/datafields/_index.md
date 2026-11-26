---
title: "PivotTable.DataFields"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает PivotFieldCollection, представляющую все поля данных в PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/datafields/
---
## PivotTable.DataFields property

Возвращает [`PivotFieldCollection`](../../pivotfieldcollection/), представляющую все поля данных в PivotTable.

```csharp
public PivotFieldCollection DataFields { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;

            // Добавить сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Получите доступ к полям данных и продемонстрируйте функциональность
            PivotFieldCollection dataFields = pivotTable.DataFields;
            if (dataFields.Count > 0)
            {
                PivotField dataField = dataFields[0];
                Console.WriteLine("Data Field Name: " + dataField.Name);
                Console.WriteLine("Data Field Function: " + dataField.Function);
            }

            // Сохраните книгу
            workbook.Save("PivotTableDataFieldsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


