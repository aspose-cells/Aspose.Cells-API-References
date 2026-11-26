---
title: "WorkbookSettings.HidePivotFieldList"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WorkbookSettings property. Получает и задаёт, скрывать ли список полей для сводной таблицы"
type: docs
url: /ru/net/aspose.cells/workbooksettings/hidepivotfieldlist/
---
## WorkbookSettings.HidePivotFieldList property

Получает и задает, скрывать ли список полей для сводной таблицы.

```csharp
public bool HidePivotFieldList { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyHidePivotFieldListDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("A");
            sheet.Cells["B4"].PutValue(150);

            // Создать сводную таблицу
            int index = workbook.Worksheets.Add(SheetType.Worksheet);
            Worksheet pivotSheet = workbook.Worksheets[index];
            pivotSheet.Name = "PivotTable";
            
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:B4", "C3");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Получите доступ к настройкам рабочей книги и задайте свойство HidePivotFieldList
            WorkbookSettings settings = workbook.Settings;
            settings.HidePivotFieldList = true; // Hide the pivot field list

            // Сохраните книгу
            workbook.Save("HidePivotFieldListDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


