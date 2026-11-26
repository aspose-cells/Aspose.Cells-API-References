---
title: "SettableGlobalizationSettings.ListSeparator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SettableGlobalizationSettings. Возвращает разделитель параметров списка функции ...etc"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/listseparator/
---
## SettableGlobalizationSettings.ListSeparator property

Получает разделитель для списка, параметров функции и т.д.

```csharp
public override char ListSeparator { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте экземпляр SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Отобразить текущее значение ListSeparator (по умолчанию запятая в большинстве локалей)
            Console.WriteLine("Current ListSeparator value: " + settings.ListSeparator);
            
            // Установить новое значение ListSeparator (например, точка с запятой)
            settings.SetListSeparator(';');
            
            // Применить настройки к рабочей книге
            workbook.Settings.GlobalizationSettings = settings;
            
            // Продемонстрировать влияние ListSeparator при разборе формулы
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue("Data");
            
            // Создать формулу, использующую разделитель списка
            worksheet.Cells["A3"].Formula = "=CONCATENATE(A1,A2)";
            
            // Формула будет использовать пользовательский разделитель списка при разборе
            Console.WriteLine("Formula with custom separator: " + worksheet.Cells["A3"].Formula);
            
            // Сохраните книгу
            workbook.Save("PropertyListSeparatorDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


