---
title: "SettableGlobalizationSettings.SetListSeparator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает разделитель для параметров списка функции ...etc"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/setlistseparator/
---
## SettableGlobalizationSettings.SetListSeparator method

Устанавливает разделитель для списка, параметров функции и т.д.

```csharp
public void SetListSeparator(char c)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| c | Char | указанный разделитель |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetListSeparatorWithCharDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // Вызовите метод SetListSeparator с параметром‑символом
                settings.SetListSeparator(';');
                
                // Применить настройки к рабочей книге
                workbook.Settings.GlobalizationSettings = settings;
                
                // Продемонстрируйте эффект, создав формулу с разделителем списка
                worksheet.Cells["A1"].Formula = "SUM(1;2;3)";
                worksheet.Cells["A2"].Value = "Formula using custom list separator: SUM(1;2;3)";
                
                Console.WriteLine("SetListSeparator method executed successfully with parameter ';'");
                Console.WriteLine("Formula using custom list separator created in cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetListSeparator method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("SetListSeparatorWithCharDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


