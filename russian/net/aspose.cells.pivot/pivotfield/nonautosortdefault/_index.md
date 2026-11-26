---
title: "PivotField.NonAutoSortDefault"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, будет ли операция сортировки, применяемая к этому полю сводной таблицы, автоматической сортировкой или простой сортировкой данных"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/nonautosortdefault/
---
## PivotField.NonAutoSortDefault property

Указывает, будет ли операция сортировки, применяемая к этому полю сводной таблицы, автоматической сортировкой или простой сортировкой данных.

```csharp
[Obsolete("Use !PivotField.SortSetting.IsSimpleSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool NonAutoSortDefault { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство !PivotField.SortSetting.IsSimpleSort. Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNonAutoSortDefaultDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получите доступ к первому листу и сводной таблице
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Получите первое поле строки в сводной таблице
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Установите свойство NonAutoSortDefault в значение true
            pivotField.NonAutoSortDefault = true;
            
            // Вывести значение свойства
            Console.WriteLine("NonAutoSortDefault property value: " + pivotField.NonAutoSortDefault);
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


