---
title: "PivotField.GroupSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Получает настройки группировки поля сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/groupsettings/
---
## PivotField.GroupSettings property

Получает настройки группировки поля сводной таблицы.

```csharp
public PivotFieldGroupSettings GroupSettings { get; }
```

### Примечания

Если это поле не сгруппировано, будет возвращено Null.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyGroupSettingsDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к первой сводной таблице.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Получите второе базовое поле (если оно существует)
            if (pivotTable.BaseFields.Count > 1)
            {
                PivotField pivotField = pivotTable.BaseFields[1];
                
                // Проверьте, имеет ли поле настройки группировки
                if (pivotField.GroupSettings != null)
                {
                    Console.WriteLine("Field has grouping enabled");
                    Console.WriteLine("Group type: " + pivotField.GroupSettings.Type);
                }
                else
                {
                    Console.WriteLine("Field has no grouping settings");
                }
                
                // Пример группировки числового поля
                if (pivotField.GroupSettings == null && 
                    pivotField.PivotItems.Count > 0 && 
                    pivotField.PivotItems[0].Value is double)
                {
                    // Группировать по числовому диапазону (интервалы по 10 единиц)
                    pivotField.GroupBy(10.0, false);
                    Console.WriteLine("Field grouped by numeric range");
                }
            }
            
            // Сохранить изменённую книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PivotFieldGroupSettings](../../pivotfieldgroupsettings/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


