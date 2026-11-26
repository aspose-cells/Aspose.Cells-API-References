---
title: "SettableGlobalizationSettings.SetBooleanValueString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает строковое представление значения булевого типа ячеек"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/setbooleanvaluestring/
---
## SettableGlobalizationSettings.SetBooleanValueString method

Устанавливает строковое значение отображения для логического значения ячейки.

```csharp
public void SetBooleanValueString(bool bv, string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| bv | Boolean | логическое значение |
| name | String | строковое представление логического значения |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetBooleanValueStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Установите пользовательские строки логических значений
            settings.SetBooleanValueString(true, "Yes");
            settings.SetBooleanValueString(false, "No");
            
            // Применить настройки к рабочей книге
            workbook.Settings.GlobalizationSettings = settings;
            
            // Установить логические значения в ячейках
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            
            // Установить стиль отображения, чтобы показывать логические значения как текст
            Style style = workbook.CreateStyle();
            style.Custom = "BOOLEAN";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A2"].SetStyle(style);
            
            try
            {
                // Сохраните книгу
                workbook.Save("SetBooleanValueStringDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean value strings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


