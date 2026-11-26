---
title: "PivotFieldCollection.AddByBaseIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFieldCollection. Добавляет объект PivotField в определённый тип PivotFields"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldcollection/addbybaseindex/
---
## PivotFieldCollection.AddByBaseIndex method

Добавляет объект PivotField в конкретный тип PivotFields.

```csharp
public int AddByBaseIndex(int baseFieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| baseFieldIndex | Int32 | Индекс поля в базовых PivotFields. |

### Возвращаемое значение

Индекс объекта PivotField в этих PivotFields.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddByBaseIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Year";
            worksheet.Cells["B2"].Value = 2022;
            worksheet.Cells["B3"].Value = 2023;
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C3", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Добавить начальные поля
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Добавить поле Year в область строк, используя AddByBaseIndex
            int newIndex = pivotTable.RowFields.AddByBaseIndex(1);
            Console.WriteLine("Added field at index: " + newIndex);

            workbook.Save("PivotFieldAddByBaseIndexDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


