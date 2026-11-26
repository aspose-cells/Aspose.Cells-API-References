---
title: "OdsSaveOptions.IgnorePivotTables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsSaveOptions. Указывает, сохраняются ли сводные таблицы"
type: docs
url: /ru/net/aspose.cells/odssaveoptions/ignorepivottables/
---
## OdsSaveOptions.IgnorePivotTables property

Указывает, сохранять ли сводные таблицы.

```csharp
public bool IgnorePivotTables { get; set; }
```

### Примечания

Функция сводных таблиц в OpenOffice имеет меньше настроек по сравнению с Excel, поэтому результаты сводных таблиц сильно различаются. Иногда лучше игнорировать эти сводные таблицы при сохранении .ods‑файла.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsSaveOptionsPropertyIgnorePivotTablesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // Создайте сводную таблицу
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Создайте экземпляр OdsSaveOptions
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // Отобразите текущее значение IgnorePivotTables
            Console.WriteLine("Current IgnorePivotTables value: " + saveOptions.IgnorePivotTables);

            // Установите игнорирование сводных таблиц при сохранении
            saveOptions.IgnorePivotTables = true;

            // Сохранить с игнорированными сводными таблицами
            workbook.Save("IgnorePivotTablesDemo_Ignored.ods", saveOptions);

            // Установите включение сводных таблиц при сохранении
            saveOptions.IgnorePivotTables = false;

            // Сохранить со включёнными сводными таблицами
            workbook.Save("IgnorePivotTablesDemo_Included.ods", saveOptions);
        }
    }
}
```

### См. также

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


