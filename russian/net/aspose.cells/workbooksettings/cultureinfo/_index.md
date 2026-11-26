---
title: "WorkbookSettings.CultureInfo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает или задает информацию о системной культуре"
type: docs
url: /ru/net/aspose.cells/workbooksettings/cultureinfo/
---
## WorkbookSettings.CultureInfo property

Получает или задает информацию о системной культуре.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Примечания

Возвращает null, если информация о культуре не установлена и [`Region`](../region/) не задана.

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            
            // Установите регион во Францию, чтобы продемонстрировать изменения CultureInfo
            wb.Settings.Region = CountryCode.France;
            
            // Получить разделитель групп из французской культуры
            string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
            Console.WriteLine($"French group separator: '{groupSep}'");
            
            // Создать стиль с пользовательским форматом и показать формат, скорректированный в соответствии с культурой
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00_ ;-#,##0.00";
            Console.WriteLine($"Culture-adjusted custom format: {style.CultureCustom}");
            
            // Продемонстрировать форматирование чисел с французской культурой
            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells["A1"];
            cell.PutValue(123456.78);
            cell.SetStyle(style);
            style.Custom = "# ###,00 €";
            
            Console.WriteLine($"Formatted value: {cell.StringValue}");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


