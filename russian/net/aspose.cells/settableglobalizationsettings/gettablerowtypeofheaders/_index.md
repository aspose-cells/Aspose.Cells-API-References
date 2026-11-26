---
title: "SettableGlobalizationSettings.GetTableRowTypeOfHeaders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает название типа строк таблицы, которые составляют заголовок таблицы. По умолчанию — Headers, поэтому в формуле Headers представляет заголовок таблицы."
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/
---
## SettableGlobalizationSettings.GetTableRowTypeOfHeaders method

Получает название типа строк таблицы, состоящих из заголовка таблицы. По умолчанию это "Headers", поэтому в формуле "#Headers" представляет заголовок таблицы.

```csharp
public override string GetTableRowTypeOfHeaders()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfHeaders("CustomHeaders");
            workbook.Settings.GlobalizationSettings = settings;

            // Создать примерные данные таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            try
            {
                // Получите тип строки таблицы для заголовков
                string rowType = settings.GetTableRowTypeOfHeaders();
                Console.WriteLine($"Table row type for headers: {rowType}");

                // Создать объект ListObject (таблица)
                ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

                // Используйте пользовательскую ссылку на заголовок в формуле
                worksheet.Cells["C2"].Formula = "=COUNTA(Table1[#CustomHeaders])";
                Console.WriteLine("Formula using custom headers reference: " + worksheet.Cells["C2"].Formula);

                // Вычислить формулу
                workbook.CalculateFormula();
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

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


