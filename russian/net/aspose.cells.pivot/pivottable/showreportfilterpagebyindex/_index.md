---
title: "PivotTable.ShowReportFilterPageByIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Показать все страницы фильтра отчёта в соответствии с индексом позиции в PageFields"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showreportfilterpagebyindex/
---
## PivotTable.ShowReportFilterPageByIndex method

Покажите все страницы фильтра отчёта в соответствии с индексом позиции в PageFields.

```csharp
public void ShowReportFilterPageByIndex(int posIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| posIndex | Int32 | Индекс позиции в PageFields |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("PivotTable.xlsx");
            
            // Получить первый лист, содержащий сводную таблицу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к первой сводной таблице.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Показать страницы фильтра отчёта по индексу (позиции) поля страницы
            int pageFieldIndex = 0; // First page field
            pivotTable.ShowReportFilterPageByIndex(pageFieldIndex);
            
            // Сохраните книгу
            workbook.Save("PivotTable_ShowReportFilterPageByIndex_Output.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


