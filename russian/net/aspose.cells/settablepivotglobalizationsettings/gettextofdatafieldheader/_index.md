---
title: "SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettablePivotGlobalizationSettings. Получает текст заголовка поля области значений в сводной таблице"
type: docs
url: /ru/net/aspose.cells/settablepivotglobalizationsettings/gettextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader method

Получает текст заголовка поля области значений в сводной таблице.

```csharp
public override string GetTextOfDataFieldHeader()
```

### Возвращаемое значение

Текст имени заголовка поля данных

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfDataFieldHeaderDemo
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
                // Получить текст по умолчанию для заголовка поля данных
                string dataFieldHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Default data field header text: {dataFieldHeaderText}");

                // Установить пользовательский текст для заголовка поля данных
                settings.SetTextOfDataFieldHeader("Custom Data Header");
                dataFieldHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Updated data field header text: {dataFieldHeaderText}");

                // Сохраните книгу
                workbook.Save("GetTextOfDataFieldHeaderDemo.xlsx");
                Console.WriteLine("GetTextOfDataFieldHeader method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfDataFieldHeader: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


