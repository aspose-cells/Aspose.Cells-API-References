---
title: "PivotTable.EnableWizard"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, доступен ли мастер сводных таблиц"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/enablewizard/
---
## PivotTable.EnableWizard property

Указывает, доступен ли мастер сводных таблиц.

```csharp
public bool EnableWizard { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableWizardDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 2000;

            // Добавьте сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Отключить мастер сводных таблиц
            pivotTable.EnableWizard = false;

            // Сохраните книгу
            workbook.Save("PivotTable_EnableWizard_Demo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


