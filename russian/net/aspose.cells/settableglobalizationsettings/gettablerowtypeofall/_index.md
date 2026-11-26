---
title: "SettableGlobalizationSettings.GetTableRowTypeOfAll"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает имя типа строк таблицы, состоящих из всех строк в ссылочной таблице"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofall/
---
## SettableGlobalizationSettings.GetTableRowTypeOfAll method

Получает название типа строк таблицы, состоящих из всех строк в ссылочной таблице.

```csharp
public override string GetTableRowTypeOfAll()
```

### Возвращаемое значение

имя типа строк таблицы

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfAllDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfAll("EntireTable");
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                string rowType = settings.GetTableRowTypeOfAll();
                Console.WriteLine($"TableRowTypeOfAll: {rowType}");

                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["A3"].Value = "Banana";
                ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "A3", true)];

                Cell formulaCell = worksheet.Cells["B1"];
                formulaCell.Formula = "=COUNTA(Table1[#All])";
                Console.WriteLine($"Formula using #All: {formulaCell.Formula}");

                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfAll method: {ex.Message}");
            }
            
            workbook.Save("MethodGetTableRowTypeOfAllDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


