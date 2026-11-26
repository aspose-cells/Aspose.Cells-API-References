---
title: "OdsLoadOptions.RefreshPivotTables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsLoadOptions. Указывает, следует ли обновлять сводные таблицы при загрузке файла"
type: docs
url: /ru/net/aspose.cells/odsloadoptions/refreshpivottables/
---
## OdsLoadOptions.RefreshPivotTables property

Указывает, следует ли обновлять сводные таблицы при загрузке файла.

```csharp
public bool RefreshPivotTables { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Создайте пример книги со сводной таблицей
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Fruit");
            sheet.Cells["A4"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Item");
            sheet.Cells["B2"].PutValue("Apple");
            sheet.Cells["B3"].PutValue("Orange");
            sheet.Cells["B4"].PutValue("Carrot");
            sheet.Cells["C1"].PutValue("Price");
            sheet.Cells["C2"].PutValue(2.5);
            sheet.Cells["C3"].PutValue(3.0);
            sheet.Cells["C4"].PutValue(1.5);

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");

            // Сохранить как ODS
            string odsPath = "output.ods";
            wb.Save(odsPath, SaveFormat.Ods);

            // Загрузите с включённым RefreshPivotTables
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            loadOptions.RefreshPivotTables = true;
            Workbook wb2 = new Workbook(odsPath, loadOptions);

            // Проверьте, что сводная таблица была обновлена
            Console.WriteLine("Pivot table count: " + wb2.Worksheets[0].PivotTables.Count);
        }
    }
}
```

### См. также

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


