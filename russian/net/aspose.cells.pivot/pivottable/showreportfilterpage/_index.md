---
title: "PivotTable.ShowReportFilterPage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Показать все страницы фильтра отчёта в соответствии с PivotField; PivotField должен находиться в PageFields"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showreportfilterpage/
---
## PivotTable.ShowReportFilterPage method

Покажите все страницы фильтра отчёта в соответствии с PivotField, PivotField должен находиться в PageFields.

```csharp
public void ShowReportFilterPage(PivotField pageField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageField | PivotField | Объект PivotField |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageWithPivotFieldDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("source.xlsx");
            
            // Доступ к первому листу и сводной таблице
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Показывать страницы фильтра отчёта для каждого поля страницы
            foreach (PivotField pageField in pivotTable.PageFields)
            {
                pivotTable.ShowReportFilterPage(pageField);
            }
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


