---
title: "SettablePivotGlobalizationSettings.GetTextOfRowLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettablePivotGlobalizationSettings. Получает текст метки Row Labels в сводной таблице"
type: docs
url: /ru/net/aspose.cells/settablepivotglobalizationsettings/gettextofrowlabels/
---
## SettablePivotGlobalizationSettings.GetTextOfRowLabels method

Получает текст метки "Row Labels" в сводной таблице.

```csharp
public override string GetTextOfRowLabels()
```

### Возвращаемое значение

Текст меток строк

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые примерные данные для контекста
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Создайте экземпляр SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Установить пользовательский текст для меток строк
                settings.SetTextOfRowLabels("Custom Row Labels");

                // Получить текст меток строк
                string rowLabelsText = settings.GetTextOfRowLabels();

                Console.WriteLine($"Text of Row Labels: {rowLabelsText}");

                // Сохраните книгу
                workbook.Save("GetTextOfRowLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfRowLabels: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


