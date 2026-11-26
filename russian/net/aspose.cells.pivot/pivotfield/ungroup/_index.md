---
title: "PivotField.Ungroup"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Разгруппировать поле сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

Разгруппировать сводное поле.

```csharp
public void Ungroup()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodUngroupDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к первой сводной таблице.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Разгруппировать первое поле столбца
            pivotTable.ColumnFields[0].Ungroup();
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


