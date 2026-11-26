---
title: "GlobalizationSettings.GetTableRowTypeOfHeaders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает имя типа строк таблицы, которые составляют заголовок таблицы. По умолчанию — Headers, поэтому в формуле Headers представляет заголовок таблицы"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/gettablerowtypeofheaders/
---
## GlobalizationSettings.GetTableRowTypeOfHeaders method

Получает название типа строк таблицы, состоящих из заголовка таблицы. По умолчанию это "Headers", поэтому в формуле "#Headers" представляет заголовок таблицы.

```csharp
public virtual string GetTableRowTypeOfHeaders()
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

    public class GlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
    {
        public class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTableRowTypeOfHeaders()
            {
                return "MyHeaders";
            }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 1.8;

            // Исправлено создание ListObject путем обработки возвращаемого значения из Add()
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            // Использовать свойство DisplayName вместо Name
            table.DisplayName = "FruitTable";

            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                worksheet.Cells["A5"].Formula = "=COUNTA(FruitTable[#MyHeaders])";
                workbook.CalculateFormula();
                Console.WriteLine("Method executed successfully. Header count: " + worksheet.Cells["A5"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfHeaders method: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


