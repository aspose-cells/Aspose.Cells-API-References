---
title: "Top10Filter.Criteria"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Top10Filter. Фактическое значение ячейки в диапазоне, которое используется для выполнения сравнения для этого фильтра. Это кэшированное значение во время процесса обновления"
type: docs
url: /ru/net/aspose.cells/top10filter/criteria/
---
## Top10Filter.Criteria property

Фактическое значение ячейки в диапазоне, которое используется для выполнения сравнения для этого фильтра. Это кэшированное значение во время процесса обновления.

```csharp
[Obsolete("Ignore this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Criteria { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, игнорируйте это свойство. Это свойство будет удалено через 12 месяцев, начиная с октября 2025 года. Компания Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class Top10FilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[i, 0].PutValue(20 - i);
            }
            
            worksheet.AutoFilter.Range = "A1:A20";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Исправление: получить доступ к свойству Filter и привести к типу Top10Filter
            Top10Filter filter = (Top10Filter)worksheet.AutoFilter.FilterColumns[0].Filter;
            Console.WriteLine("Current Criteria value: " + filter.Criteria);
            
            filter.Criteria = 14;
            
            worksheet.AutoFilter.Refresh();
            
            workbook.Save("Top10FilterCriteriaDemo.xlsx");
        }
    }
}
```

### См. также

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


