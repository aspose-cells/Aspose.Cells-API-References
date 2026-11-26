---
title: "PivotFieldCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFieldCollection. Добавляет объект PivotField в определённый тип PivotFields"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldcollection/add/
---
## PivotFieldCollection.Add method

Добавляет объект PivotField в конкретный тип PivotFields.

```csharp
public int Add(PivotField pivotField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotField | PivotField | Объект PivotField. |

### Возвращаемое значение

Индекс объекта PivotField в этих PivotFields.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddWithPivotFieldDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("sample_pivot_table.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к первой сводной таблице.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Обновить данные сводной таблицы
            pivotTable.RefreshData();
            
            // Добавить поле данных в область столбцов, используя метод Add
            pivotTable.ColumnFields.Add(pivotTable.DataField);
            
            // Вычислить данные сводной таблицы
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("output_pivot_table.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


