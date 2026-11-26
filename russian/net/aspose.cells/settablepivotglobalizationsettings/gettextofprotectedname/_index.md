---
title: "SettablePivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettablePivotGlobalizationSettings. Получает текст для указанного защищённого имени"
type: docs
url: /ru/net/aspose.cells/settablepivotglobalizationsettings/gettextofprotectedname/
---
## SettablePivotGlobalizationSettings.GetTextOfProtectedName method

Получает текст для указанного защищённого имени.

```csharp
public override string GetTextOfProtectedName(string protectedName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| protectedName | String | Защищённое имя в сводной таблице. |

### Возвращаемое значение

Локальные защищённые имена сводной таблицы.

### Примечания

В Microsoft Excel некоторые имена нельзя использовать в качестве названий полей PivotFields в сводной таблице. Они различаются в разных регионах, пользователь может явно указать их в соответствии с используемым регионом.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые примерные данные для контекста
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Создайте экземпляр SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Установить пользовательский текст для защищённого имени
                settings.SetTextOfProtectedName("Sum", "Total Sum");

                // Получить текст защищённого имени
                string protectedNameText = settings.GetTextOfProtectedName("Sum");

                Console.WriteLine($"Text for protected name 'Sum': {protectedNameText}");

                // Сохраните книгу
                workbook.Save("GetTextOfProtectedNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


