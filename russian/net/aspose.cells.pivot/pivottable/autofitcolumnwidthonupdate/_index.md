---
title: "PivotTable.AutofitColumnWidthOnUpdate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, следует ли автоматически подгонять ширину столбца при обновлении"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/
---
## PivotTable.AutofitColumnWidthOnUpdate property

Указывает, следует ли автоматически подгонять ширину столбца при обновлении

```csharp
public bool AutofitColumnWidthOnUpdate { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutofitColumnWidthOnUpdateDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получить доступ к листу, содержащему сводную таблицу
            Worksheet worksheet = workbook.Worksheets["PIVOT"];
            
            // Получить доступ к сводной таблице
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Отключить автоматическую подгонку ширины столбца при обновлении
            pivotTable.AutofitColumnWidthOnUpdate = false;
            
            // Обновить сводную таблицу, чтобы применить изменения
            worksheet.RefreshPivotTables();
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            Console.WriteLine("PivotTable AutofitColumnWidthOnUpdate property set successfully.");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


