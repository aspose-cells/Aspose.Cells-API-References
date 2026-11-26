---
title: "SettableGlobalizationSettings.GetErrorValueString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает строковое представление значения ошибки ячеек"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/geterrorvaluestring/
---
## SettableGlobalizationSettings.GetErrorValueString method

Получает отображаемое строковое значение ошибки ячейки.

```csharp
public override string GetErrorValueString(string err)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ошибка | String | значения ошибок, такие как #VALUE!,#NAME? |

### Возвращаемое значение

По умолчанию возвращает само значение ошибки

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetErrorValueStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Создать ячейку с значением ошибки
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("#N/A");
            Style style = workbook.CreateStyle();
            cell.SetStyle(style);
            style.Number = 10; // Set format to Error value

            try
            {
                // Вызвать GetErrorValueString со строкой значения ошибки
                string errorString = settings.GetErrorValueString("#N/A");
                
                // Отобразить результат
                Console.WriteLine("Error value string: " + errorString);

                // Показать эффект, установив значение другой ячейки в возвращённую строку
                worksheet.Cells["A2"].PutValue("Error representation: " + errorString);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


