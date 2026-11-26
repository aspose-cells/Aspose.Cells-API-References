---
title: "PivotGlobalizationSettings.GetTextOfQuarters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает локальный текст Quarters"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/
---
## PivotGlobalizationSettings.GetTextOfQuarters method

Получите локальный текст "Quarters".

```csharp
public virtual string GetTextOfQuarters()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfQuartersDemo
    {
        public static void Run()
        {
            // Создайте экземпляр настроек глобализации
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Продемонстрируйте метод GetTextOfQuarters
            Console.WriteLine("Quarter labels: " + globalizationSettings.GetTextOfQuarters());
            
            // Покажите другие связанные метки временных периодов для контекста
            Console.WriteLine("Year labels: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Month labels: " + globalizationSettings.GetTextOfMonths());
        }
    }
}
```

### См. также

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


