---
title: "PivotField.Position"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Представляет индекс PivotField в области"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/position/
---
## PivotField.Position property

Представляет индекс [`PivotField`](../) в области.

```csharp
public int Position { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPositionDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook wb = new Workbook("NET46429_a.xlsx");
            
            // Получите доступ к первому листу и его сводной таблице
            Worksheet ws = wb.Worksheets[0];
            PivotTable pt = ws.PivotTables[0];
            
            // Продемонстрировать использование свойства Position
            int position = pt.PageFields[0].Position;
            Console.WriteLine("Position of first page field: " + position);
            
            // Используйте position для отображения страниц фильтра отчёта
            pt.ShowReportFilterPageByIndex(position);
            
            // Сохраните книгу
            wb.Save("PivotFieldPropertyPositionDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


