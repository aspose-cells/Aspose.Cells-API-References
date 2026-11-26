---
title: "PivotGlobalizationSettings.GetShortTextOf12Months"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает все коротко отформатированные строки для 12 месяцев"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/
---
## PivotGlobalizationSettings.GetShortTextOf12Months method

Получает все коротко отформатированные строки 12 месяцев.

```csharp
public virtual string[] GetShortTextOf12Months()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetShortTextOf12MonthsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пользовательский класс настроек глобализации, наследующий от PivotGlobalizationSettings
            var customGlobalizationSettings = new CustomPivotGlobalizationSettings();

            try
            {
                // Вызовите метод GetShortTextOf12Months
                string[] monthShortNames = customGlobalizationSettings.GetShortTextOf12Months();

                // Выведите названия месяцев в консоль
                Console.WriteLine("Short names of 12 months:");
                foreach (string monthName in monthShortNames)
                {
                    Console.WriteLine(monthName);
                }

                // Добавьте названия месяцев в лист
                for (int i = 0; i < monthShortNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(monthShortNames[i]);
                }

                Console.WriteLine("Method executed successfully. Month names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetShortTextOf12Months method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("MethodGetShortTextOf12MonthsDemo.xlsx");
        }
    }

    // Пользовательская реализация PivotGlobalizationSettings для переопределения GetShortTextOf12Months
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetShortTextOf12Months()
        {
            // Верните пользовательские короткие названия месяцев
            return new string[] { "Jan", "Feb", "Mar", "Apr", "May", "Jun", 
                                "Jul", "Aug", "Sep", "Oct", "Nov", "Dec" };
        }
    }
}
```

### См. также

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


