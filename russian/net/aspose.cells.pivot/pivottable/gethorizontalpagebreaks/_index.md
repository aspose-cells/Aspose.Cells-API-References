---
title: "PivotTable.GetHorizontalPageBreaks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Получает горизонтальные разрывы страниц этой сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/gethorizontalpagebreaks/
---
## PivotTable.GetHorizontalPageBreaks method

Получает горизонтальные разрывы страниц этой сводной таблицы.

```csharp
public int[] GetHorizontalPageBreaks()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу из исходного файла
            Workbook workbook = new Workbook("pivot_pagebreaks.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к первой сводной таблице.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Обновить и вычислить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Получить горизонтальные разрывы страниц
            int[] pageBreaks = pivotTable.GetHorizontalPageBreaks();
            
            // Отобразите результаты
            Console.WriteLine("Horizontal Page Breaks:");
            foreach (int row in pageBreaks)
            {
                Console.WriteLine("Row: " + row);
            }
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


