---
title: "WorkbookSettings.LanguageCode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает или задает язык пользовательского интерфейса версии книги на основе CountryCode, в котором файл был сохранён"
type: docs
url: /ru/net/aspose.cells/workbooksettings/languagecode/
---
## WorkbookSettings.LanguageCode property

Получает или задает язык пользовательского интерфейса версии Workbook, основанный на CountryCode, который сохранил файл.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;

            // Установите код языка на German (Germany)
            settings.LanguageCode = CountryCode.Germany;

            // Отобразите текущий код языка
            Console.WriteLine("Current Language Code: " + settings.LanguageCode);

            // Измените код языка на French (France)
            settings.LanguageCode = CountryCode.France;
            Console.WriteLine("Updated Language Code: " + settings.LanguageCode);

            // Сохраните книгу
            workbook.Save("WorkbookSettings_LanguageCodeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


