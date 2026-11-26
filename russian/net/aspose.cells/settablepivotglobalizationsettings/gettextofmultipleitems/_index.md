---
title: "SettablePivotGlobalizationSettings.GetTextOfMultipleItems"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettablePivotGlobalizationSettings. Получает текст метки Multiple Items в сводной таблице"
type: docs
url: /ru/net/aspose.cells/settablepivotglobalizationsettings/gettextofmultipleitems/
---
## SettablePivotGlobalizationSettings.GetTextOfMultipleItems method

Получает текст метки "(Multiple Items)" в сводной таблице.

```csharp
public override string GetTextOfMultipleItems()
```

### Возвращаемое значение

Текст метки "(Multiple Items)"

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
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
                // Получить текст по умолчанию для нескольких элементов
                string multipleItemsText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Default text for multiple items: {multipleItemsText}");

                // Установить пользовательский текст для нескольких элементов
                settings.SetTextOfMultipleItems("(Multiple Items Custom)");
                multipleItemsText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Updated text for multiple items: {multipleItemsText}");

                // Сохраните книгу
                workbook.Save("GetTextOfMultipleItemsDemo.xlsx");
                Console.WriteLine("GetTextOfMultipleItems method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


